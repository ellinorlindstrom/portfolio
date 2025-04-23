<script>
	import { css } from 'styled-system/css';
</script>

<section class="hero">
	<div class="introduction">
		<h1 class={css({ fontSize: '2.625rem' }) + ' text-h1'}>Hi, I'm Ellinor Lindström,</h1>
		<p class="p-medium">
			A developer based in Malmö, Sweden. I'm specialized in frontend development, with a passion
			for UX/UI, creating clean, accessible and delightful digital experiences, blending technical
			expertise with creative problem-solving.
		</p>
		<button class="btn btn-primary text-p-small">Read more!</button>
	</div>
	<a href="/about">
		<div class="image-container">
			<img
				src="../icons/portfolio-portrait.png"
				alt="A portrait of Ellinor Lindström"
				width="500"
				height="auto"
				loading="lazy"
				class="image primary"
			/>
			<img
				src="../icons/portfolio-portrait-hover.png"
				alt="A portrait of Ellinor Lindström"
				width="500"
				height="auto"
				loading="lazy"
				class="image hover"
			/>
		</div>
	</a>
</section>

<style>
	.hero {
		display: flex;
		flex-direction: row;
		align-items: flex-start;
		text-align: left;
		padding: 2rem 1rem;
	}

	.introduction {
		padding-top: 100px;
	}

	.image-container {
		position: relative;
		width: 350px;
	}

	.image {
		width: 100%;
		height: auto;
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
</style>
