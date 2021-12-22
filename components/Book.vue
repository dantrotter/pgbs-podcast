<template>
		<div>
				<h1>{{ name.toUpperCase() }}</h1>
				<ol>
						<li v-for="chapter in books[name.toLowerCase()]" :key="chapter">
							<h2>Chapter {{ chapter.chapter }}</h2>
							<ol>
								<li v-for="study in chapter.studies" :key="study.title">
									{{ study.title }} - <a :href="study.audio">audio</a> - <a :href="study.outline">outline</a>
								</li>
							</ol>
						</li>
				</ol>
		</div>
</template>

<script>
	import genesis from '/data/genesis';
	import james from '/data/james';
	
	export default {
			name: 'Book',
			props: {
					name: {
							type: String,
							default: null
					}
			},
			data(){
				return {
					books: { genesis, james }
				}
			}
	}
</script>

<style lang="scss" scoped>

</style>