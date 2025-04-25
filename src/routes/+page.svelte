<script>
	import Footer from '../components/Footer.svelte';
	import Header from '../components/Header.svelte';
	import Hero from '../components/Hero.svelte';
	import Projects from '../components/Projects.svelte';
</script>

<div class="layout-container">
	<Header />
	<Hero />
	<Projects />
	<Footer />
</div>

<style>
	@media (min-width: 769px) {
		.layout-container {
			position: relative;
		}

		:global(.hero) {
			position: relative;
			z-index: 2;
			margin-bottom: -250px;
			padding-bottom: 100px;
		}
		:global(.projects-container) {
			position: relative;
			z-index: 1;
		}
	}
</style>
