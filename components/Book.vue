<template>
		<div>
				<h1>{{ friendlyName }}</h1>
				<ol>
						<li v-for="chapter in books[friendlyName]" :key="chapter">
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
	import books from '/data/books';
	
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
					books: books,
					friendlyName: this.name.replace(/-/g, ' ').replace(/(^\w|\s\w)/g, w => w.toUpperCase())
				}
			}
	}
</script>

<style lang="scss" scoped>

</style>