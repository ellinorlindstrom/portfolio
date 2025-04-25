<script>
	import { css } from 'styled-system/css';
	import { browser } from '$app/environment';
	import { onMount } from 'svelte';

	let isMobile = false;

	onMount(() => {
		if (browser) {
			const checkMobile = () => window.innerWidth <= 768;
			isMobile = checkMobile();

			window.addEventListener('resize', () => {
				isMobile = checkMobile();
			});
		}
	});
</script>

<section class="hero">
	<div class="introduction">
		<h1 class={css({ fontSize: '2.625rem' }) + ' text-h1'}>Hi, I'm Ellinor,</h1>
		<p class="p-medium">
			Welcome to my code-gallery. I'm a developer based in Malmö, Sweden, with an enthusiasm for
			UX/UI design and a strong desire to learn.
		</p>
		<a href="/about" class="btn btn-primary text-p-small">Read more!</a>
	</div>
	{#if !isMobile}
		<a href="/about">
			<div class="image-container">
				<img
					src="../icons/portrait.png"
					alt="A portrait of Ellinor Lindström"
					width="500"
					height="auto"
					loading="lazy"
					class="image primary"
				/>
				<img
					src="../icons/portrait-hover.png"
					alt="A portrait of Ellinor Lindström"
					width="500"
					height="auto"
					loading="lazy"
					class="image hover"
				/>
			</div>
		</a>
	{/if}
</section>

<style>
	.hero {
		display: flex;
		flex-direction: row;
		align-items: flex-start;
		text-align: left;
		padding: 2rem 0 0 0;
	}

	.image-container {
		position: relative;
		width: 350px;
	}

	.image {
		width: 100%;
		height: auto;
		margin-left: 100px;
	}

	.hover {
		position: absolute;
		top: 0;
		left: 0;
		opacity: 0;
	}

	.image-container:hover .hover {
		opacity: 1;
	}
	.image-container:hover .primary {
		opacity: 0;
	}

	a.btn {
		display: inline-block;
		text-decoration: none;
	}
</style>
