<script lang="ts">
	import '../styles/index.css';
	import 'styled-system/css';

	let { children } = $props();
</script>

<div class="layout-container">
	{@render children()}
</div>

<style>
	.layout-container {
		max-width: 1200px;
		margin: 0 auto;
		padding: 2rem 1rem;
	}
</style>
