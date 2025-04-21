<script>
	import { css } from 'styled-system/css';
</script>

<h2 class="section-heading">Projects</h2>
<div class="projects-container">
	<div class="frame-container">
		<a href="https://starwarsfunkyclopedia.netlify.app/" target="_blank" rel="noopener noreferrer">
			<img
				src="../projects/star-wars-framed.png"
				alt="Star wars encyclopedia project"
				loading="lazy"
				class="frame"
			/>
		</a>
		<h3 class="project-title">Star Wars Encyclopedia</h3>
		<p class="project-description">
			School project. All things Star Wars—films, characters, planets, starships, and more, built in
			react.
		</p>
	</div>
	<div class="frame-container">
		<a href="https://popcornparadise.netlify.app/" target="_blank" rel="noopener noreferrer">
			<img
				src="../projects/movie-db-framed.png"
				alt="Popcorn paradise movie database project"
				loading="lazy"
				class="frame"
			/>
		</a>
		<h3 class="project-title">Movie Database</h3>
		<p class="project-description">
			School project. All your latest, most popular and top rated movies in one place, built in
			react.
		</p>
	</div>
	<div class="frame-container">
		<a href="https://lollyland-express.netlify.app/" target="_blank" rel="noopener noreferrer">
			<img
				src="../projects/candy-shop-framed.png"
				alt="Lollyland express candy shop project"
				loading="lazy"
				class="frame"
			/>
		</a>
		<h3 class="project-title">Candy Shop</h3>
		<p class="project-description">Candy shop built with two of my classmates using JS. Indulge!</p>
	</div>
	<div class="frame-container">
		<a href="https://country-flag-quiz.netlify.app/" target="_blank" rel="noopener noreferrer">
			<img src="../projects/quiz-framed.png" alt="Flag quiz project" loading="lazy" class="frame" />
		</a>
		<h3 class="project-title">Flaq Quiz</h3>
		<p class="project-description">
			Interactive challenge originally featuring classmates, exchanged for a flag-country matching
			game, using HTML, CSS, and JS for collaborative learning.
		</p>
	</div>
	<div class="frame-container">
		<a href="https://vimeo.com/1076489845?share=copy" target="_blank" rel="noopener noreferrer">
			<img
				src="../projects/sq-framed.png"
				alt="Stride quest project"
				loading="lazy"
				class="frame"
			/>
		</a>
		<h3 class="project-title">Stride quest</h3>
		<p class="project-description">
			An iOS application created using Swift that transforms users' real-world fitness activities
			into virtual journeys on a map, making exercise more engaging and a learning experience. I
			learned a lot from this project. Especially the importance of thorough planning, something I
			would've spent more time of if I were to do this again.
		</p>
	</div>
</div>

<style>
	.section-heading {
		text-align: center;
		padding: 2rem 0;
		width: 100%;
	}
	.projects-container {
		display: grid;
		grid-template-columns: 1fr;
		gap: 2rem;
		text-align: center;
		margin: 0 auto;
		max-width: 1000%;
	}

	.frame-container {
		display: flex;
		flex-direction: column;
		align-items: center;
		position: relative;
		width: 100%;
		max-width: 600px;
		margin: 0 auto;
	}

	.frame {
		position: relative;
		max-width: 100%;
	}
	.frame-container:nth-child(n) {
		grid-column: 1;
		grid-row: auto;
	}

	@media (min-width: 769px) {
		.projects-container {
			grid-template-columns: repeat(2, 1fr);
			grid-template-rows: auto auto auto;
			max-width: 1200px;
		}

		.frame-container:nth-child(1) {
			grid-column: 1;
			grid-row: 1;
		}

		.frame-container:nth-child(2) {
			grid-column: 2;
			grid-row: 1;
		}

		.frame-container:nth-child(3) {
			grid-column: 1;
			grid-row: 2;
		}

		.frame-container:nth-child(4) {
			grid-column: 1;
			grid-row: 3;
		}

		.frame-container:nth-child(5) {
			grid-column: 2;
			grid-row: 2 / span 2;
		}
	}
</style>
