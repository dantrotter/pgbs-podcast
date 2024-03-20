<template>
	<div class="bible-menu">
		<button on="tap:sidebar.open" class="bible-menu__button">STUDY NOTES and audio here</button>
		<amp-sidebar id="sidebar" layout="nodisplay" side="right">
			<nav>
				<amp-accordion animate expand-single-section>

					<section>
						<h2>Old Testament</h2>
						<ol>
							<li><NuxtLink to="/genesis">Genesis</NuxtLink></li>
							<li><NuxtLink to="/exodus">Exodus</NuxtLink></li>
							<li><NuxtLink to="/leviticus">Leviticus</NuxtLink></li>
							<li><NuxtLink to="/numbers">Number</NuxtLink></li>
							<li><NuxtLink to="/deuteronomy">Deuteronomy</NuxtLink></li>
							<li><NuxtLink to="/joshua">Joshua</NuxtLink></li>
							<li><NuxtLink to="/judges">Judges</NuxtLink></li>
							<li><NuxtLink to="/ruth">Ruth</NuxtLink></li>
							<li><NuxtLink to="/1-samuel">1 Samuel</NuxtLink></li>
							<li><NuxtLink to="/2-samuel">2 Samuel</NuxtLink></li>
							<li><NuxtLink to="/1-kings">1 Kings</NuxtLink></li>
							<li><NuxtLink to="/2-kings">2 Kings</NuxtLink></li>
							<li><NuxtLink to="/ezra">Ezra</NuxtLink></li>
							<li><NuxtLink to="/nehemiah">Nehemiah</NuxtLink></li>
							<li><NuxtLink to="/esther">Esther</NuxtLink></li>
							<li><NuxtLink to="/job">Job</NuxtLink></li>
							<li><NuxtLink to="/psalms">Psalms</NuxtLink></li>
							<li><NuxtLink to="/proverbs">Proverbs</NuxtLink></li>
							<li><NuxtLink to="/ecclesiastes">Ecclesiastes</NuxtLink></li>
							<li><NuxtLink to="/song-of-solomon">Song of Solomon</NuxtLink></li>
							<li><NuxtLink to="/isaiah">Isaiah</NuxtLink></li>
							<li><NuxtLink to="/Jeremiah">Jeremiah</NuxtLink></li>
							<li><NuxtLink to="/lamentations">Lamentations</NuxtLink></li>
							<li><NuxtLink to="/ezekiel">Ezekiel</NuxtLink></li>
							<li><NuxtLink to="/daniel">Daniel</NuxtLink></li>
							<li><NuxtLink to="/hosea">Hosea</NuxtLink></li>
							<li><NuxtLink to="/joel">Joel</NuxtLink></li>
							<li><NuxtLink to="/amos">Amos</NuxtLink></li>
							<li><NuxtLink to="/obadiah">Obadiah</NuxtLink></li>
							<li><NuxtLink to="/jonah">Jonah</NuxtLink></li>
							<li><NuxtLink to="/micah">Micah</NuxtLink></li>
							<li><NuxtLink to="/nahum">Nahum</NuxtLink></li>
							<li><NuxtLink to="/habakkuk">Habakkuk</NuxtLink></li>
							<li><NuxtLink to="/zephaniah">Zephaniah</NuxtLink></li>
							<li><NuxtLink to="/haggai">Haggai</NuxtLink></li>
							<li><NuxtLink to="/zechariah">Zechariah</NuxtLink></li>
							<li><NuxtLink to="/malachi">Malachi</NuxtLink></li>
						</ol>
					</section>
					<section expanded>
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