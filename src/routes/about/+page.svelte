<script>
	import Footer from '../../components/Footer.svelte';
	import Header from '../../components/Header.svelte';
</script>

<div class="layout-container">
	<Header />
	<section class="about">
		<h2 class="section-heading">About</h2>
		<section class="about-text-image">
			<p class="section-description">
				I'm a front-end developer with a passion for creating beautiful and functional user
				interfaces. I love to learn new things within web development. I have experience with HTML,
				CSS, JavaScript, React, Svelte, and Three.js. I'm always looking for new challenges and
				opportunities to grow as a developer. In my free time, I enjoy reading books, coding,
				painting/drawing/creative projects, working out, and spending time with my family and
				friends.
			</p>
			<img
				src="../icons/about.png"
				alt="Portrait photagraphy of Ellinor Lindström"
				width="300"
				height="auto"
				loading="lazy"
				class="about-image"
			/>
		</section>
	</section>
	<Footer />
</div>

<style>
	.layout-container {
		display: flex;
		flex-direction: column;
		height: 100vh;

		padding-top: 0;
	}

	.about {
		flex: 1;
		display: flex;
		flex-direction: column;
		text-align: left;
		padding: 4rem 1rem;
	}

	.about-text-image {
		display: flex;
		flex-direction: column;
		gap: 1.5rem;
		align-items: center;
	}

	.section-description {
		width: 100%;
	}

	.about-image {
		width: 100%;
		max-width: 250px;
		height: auto;
	}

	@media (min-width: 768px) {
		.about-text-image {
			flex-direction: row;
			gap: 2rem;
			align-items: flex-start;
		}

		.section-description {
			flex: 1;
		}

		.about-image {
			max-width: 300px;
		}
	}
</style>
