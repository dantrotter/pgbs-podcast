<template>
	<div>
		<button on="tap:sidebar.open">Menu</button>
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
							<li><NuxtLink to="/james">James</NuxtLink></li>
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