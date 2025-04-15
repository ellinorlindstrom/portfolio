<script>
	import ThemeToggle from './ThemeToggle.svelte';
	import Logo from './Logo.svelte';
</script>

<header>
	<div class="container">
		<div class="logo-container">
			<Logo />
		</div>
		<div class="toggle-container">
			<ThemeToggle />
		</div>
	</div>
</header>

<style>
	header {
		width: 100%;
		padding: 1rem 0;
	}

	.container {
		max-width: 1200px;
		margin: 0 auto;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0 1rem;
	}

	.logo-container {
		/* Adjust as needed */
	}

	.toggle-container {
		/* Adjust as needed */
	}
</style>
