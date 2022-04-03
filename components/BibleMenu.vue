<template>
	<div class="bible-menu">
		<button on="tap:sidebar.open" class="bible-menu__button">find audio and notes by book</button>
		<amp-sidebar id="sidebar" layout="nodisplay" side="right">
			<nav>
				<amp-accordion animate expand-single-section>
					<section>
						<h2>Old Testament</h2>
						<amp-accordion animate expand-single-section>
							<section>
							<h3>Pentateuch</h3>
							<ol>
								<li><NuxtLink to="/genesis">Genesis</NuxtLink></li>
								<li><NuxtLink to="/exodus">Exodus</NuxtLink></li>
								<li><NuxtLink to="/leviticus">Leviticus</NuxtLink></li>
								<li><NuxtLink to="/numbers">Number</NuxtLink></li>
								<li><NuxtLink to="/deuteronomy">Deuteronomy</NuxtLink></li>
							</ol>
							</section>
							<section>
							<h3>Prophets</h3>
							<ol>
								<li><NuxtLink to="/isaiah">Isaiah</NuxtLink></li>
								<li><NuxtLink to="/ezekiel">Ezekiel</NuxtLink></li>
							</ol>
							</section>
						</amp-accordion>
					</section>
					<section>
						<h2>New Testament</h2>
						<ol>
							<li><NuxtLink to="/matthew">Matthew</NuxtLink></li>
							<li><NuxtLink to="/mark">Mark</NuxtLink></li>
							<li><NuxtLink to="/luke">Luke</NuxtLink></li>
							<li><NuxtLink to="/john">John</NuxtLink></li>
							<li><NuxtLink to="/acts">Acts</NuxtLink></li>
							<li><NuxtLink to="/romans">Romans</NuxtLink></li>
							<li><NuxtLink to="/1-corinthians">1 Corinthians</NuxtLink></li>
							<li><NuxtLink to="/2-corinthians">2 Corinthians</NuxtLink></li>
							<li><NuxtLink to="/galatians">Galatians</NuxtLink></li>
							<li><NuxtLink to="/ephesians">Ephesians</NuxtLink></li>
							<li><NuxtLink to="/philippians">Philippians</NuxtLink></li>
							<li><NuxtLink to="/colossians">Colossians</NuxtLink></li>
							<li><NuxtLink to="/1-thessalonians">1 Thessalonians</NuxtLink></li>
							<li><NuxtLink to="/2-thessalonians">2 Thessalonians</NuxtLink></li>
							<li><NuxtLink to="/1-timothy">1 Timothy</NuxtLink></li>
							<li><NuxtLink to="/2-timothy">2 Timothy</NuxtLink></li>
							<li><NuxtLink to="/titus">Titus</NuxtLink></li>
							<li><NuxtLink to="/philemon">Philemon</NuxtLink></li>
							<li><NuxtLink to="/hebrews">Hebrews</NuxtLink></li>
							<li><NuxtLink to="/james">James</NuxtLink></li>
							<li><NuxtLink to="/1-peter">1 Peter</NuxtLink></li>
							<li><NuxtLink to="/2-peter">2 Peter</NuxtLink></li>
							<li><NuxtLink to="/1-john">1 John</NuxtLink></li>
							<li><NuxtLink to="/2-john">2 John</NuxtLink></li>
							<li><NuxtLink to="/3-john">3 John</NuxtLink></li>
							<li><NuxtLink to="/jude">Jude</NuxtLink></li>
							<li><NuxtLink to="/revelation">Revelation</NuxtLink></li>
						</ol>
					</section>
				</amp-accordion>
			</nav>
		</amp-sidebar>
	</div>
</template>

<script>
	export default {
		name: 'Menu'
	}
</script>