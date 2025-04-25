<script>
	import Footer from '../../components/Footer.svelte';
	import Header from '../../components/Header.svelte';
</script>

<div class="layout-container">
	<Header />
	<section class="about">
		<h1>About me</h1>
		<section class="about-text-image">
			<div class="about-text">
				<p class="section-description">
					My journey to web development has been driven by curiosity and a strong desire to grow.
					What drives me forward is my determination to transform ideas into reality and my
					willingness to tackle challenges, even when the path isn't straightforward.
				</p>
				<h2 class="section-heading">Education</h2>
				<p class="section-description">
					I graduated from <a
						href="https://medieinstitutet.se/utbildningar/front-end-developer/"
						target="_blank"
						rel="noopener noreferrer"
					>
						Mediainstitutet
					</a>
					in Malmö, Sweden in spring 2025, where I developed skills in subjects such as TypeScript, React,
					Svelte(from my intenship at
					<a href="https://www.coolstuff.se/" target="_blank" rel="noopener noreferrer">
						Coolstuff)</a
					> and UX/UI design. Though my formal education is complete, I'm committed to continuous learning
					and regularly work on personal projects to expand my capabilities.
				</p>
				<h2 class="section-heading">Work</h2>
				<p class="section-description">
					I'm starting a new position as Customer Solutions and UX Coordinator at <a
						href="https://www.glimja.com/"
						target="_blank"
						rel="noopener noreferrer">Glimja</a
					>
					and
					<a href="https://www.happygreen.se/" target="_blank" rel="noopener noreferrer"
						>Happy green</a
					> where I'll be developing with Svelte and leading initiatives to enhance user experience across
					both B2C and B2B platforms. My focus will be on improving conversion rates, customer lifetime
					value, and overall satisfaction through data-driven UX improvements.
				</p>
				<h2 class="section-heading">Hobbies</h2>
				<p class="section-description">
					Outside of work, I cherish time with family and friends, enjoy diving into good books, and
					maintain an active lifestyle. Currently, I'm exploring different art forms, particularly
					digital illustration, oil painting, watercolor, and traditional sketching, which helps me
					develop a better eye for design in my professional work.
				</p>
			</div>

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
		padding: 2rem 0;
	}

	.about-text-image {
		display: flex;
		flex-direction: column;
		gap: 1.5rem;
		align-items: center;
	}

	.section-heading {
		font-size: 1.15rem;
		margin: 1rem 0 0.5rem 0;
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
