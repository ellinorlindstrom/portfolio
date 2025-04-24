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
	.layout-container {
		padding-top: 0;
	}
</style>
