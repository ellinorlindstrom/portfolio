<script>
	import { browser } from '$app/environment';
	import { onMount } from 'svelte';

	let isDarkMode = false;

	const toggleTheme = () => {
		isDarkMode = !isDarkMode;
		document.body.classList.toggle('dark', isDarkMode);
		if (browser) {
			localStorage.setItem('theme', isDarkMode ? 'dark' : 'light');
		}
	};

	onMount(() => {
		if (browser) {
			const currentTheme = localStorage.getItem('theme');
			if (currentTheme === 'dark') {
				isDarkMode = true;
				document.body.classList.add('dark');
			}
		}
	});
</script>

<button on:click={toggleTheme} aria-label="Toggle theme">
	{#if isDarkMode}
		<img src="/icons/moon.png" alt="Moon icon" />
	{:else}
		<img src="/icons/sun.png" alt="Sun icon" />
	{/if}
</button>

<style>
	button {
		width: 25px;
		height: 25px;
		background: none;
		border: none;
		cursor: pointer;
		font-size: 1.5rem;
	}
</style>
