<script>
	/* 	import ThemeToggle from './ThemeToggle.svelte';
	 */ import Logo from './Logo.svelte';
</script>

<header>
	<div class="container">
		<div class="logo-container">
			<Logo />
		</div>
		<!-- <div class="toggle-container">
			<ThemeToggle />
		</div> -->
	</div>
</header>

<style>
	.container {
		display: flex;
		justify-content: space-between;
		align-items: center;
	}
</style>
