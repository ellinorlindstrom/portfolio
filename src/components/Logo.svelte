<script>
	export let logoUrl = '../icons/EL-icon.png';
</script>

<div class="logo">
	<a href="/">
		<img src={logoUrl} alt="Logo" />
	</a>
</div>

<style>
	.logo {
		display: flex;
		align-items: flex-start;
	}

	.logo img {
		max-width: 50px;
		height: auto;
	}
</style>
