<script>
	import { css } from 'styled-system/css';
</script>

<section class="hero">
	<div class="introduction">
		<h1 class={css({ fontSize: '2.625rem' }) + ' text-h1'}>Hi, I'm Ellinor Lindström,</h1>
		<p class="p-medium">
			A developer based in Malmö, Sweden. I'm specialized in frontend development, with a passion
			for UX/UI and creating clean, accessible and delightful digital experiences, blending
			technical expertise with creative problem-solving.
		</p>
		<button class="btn btn-primary">Read more!</button>
	</div>
	<img
		src="../icons/portfolio-portrait.png"
		alt="A portrait of Ellinor Lindström"
		width="500"
		height="auto"
		loading="lazy"
		class="image"
	/>
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
</style>
