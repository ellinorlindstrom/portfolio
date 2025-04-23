<script>
	import Footer from '../../components/Footer.svelte';
	import Header from '../../components/Header.svelte';
</script>

<Header />
<div class="layout-container">
	<section class="about-text">
		<h2 class="section-heading">About</h2>
		<section class="about">
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
	}
	.about-text {
		display: flex;
		flex-direction: column;
		text-align: left;
	}

	.about {
		display: flex;
		flex-direction: row;
		gap: 2rem;
	}
</style>
