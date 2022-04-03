<template>
		<main>
				<h1 class="book-header">{{ friendlyName }}</h1>
				<ol class="book-list">
						<li v-for="chapter in books[friendlyName]" :key="chapter">
							<h2 class="small-header">Chapter {{ chapter.chapter }}</h2>
							<ul>
								<li v-for="study in chapter.studies" :key="study.title">
									{{ study.title }} - <a :href="study.audio" target="_blank">audio</a> - <a :href="study.outline">outline</a>
								</li>
							</ul>
						</li>
				</ol>
	</main>
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