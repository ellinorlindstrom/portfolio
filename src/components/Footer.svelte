<script>
	const currentYear = new Date().getFullYear();
</script>

<footer>
	<section class="social-icons">
		<a href="mailto:lindstrom.elle@gmail.com" aria-label="Email">
			<img src="../icons/mail.png" alt="mail icon" width="30" height="30" />
		</a>
		<a
			href="https://github.com/ellinorlindstrom"
			target="_blank"
			rel="noopener noreferrer"
			aria-label="GitHub"
		>
			<img src="../icons/github.png" alt="github icon" width="30" height="30" />
		</a>
		<a
			href="https://www.linkedin.com/in/ellinor-amanda-lindstrom/"
			target="_blank"
			rel="noopener noreferrer"
			aria-label="LinkedIn"
		>
			<img src="../icons/linkedin.png" alt="linkedin icon" width="30" height="30" />
		</a>
	</section>
	<p>©{currentYear} Ellinor Lindström</p>
</footer>

<style>
	.social-icons {
		display: flex;
		justify-content: center;
		gap: 1rem;
		margin-bottom: 0.5rem;
	}
	footer {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		color: var(--text-color);
		font-size: 1rem;
		padding: 5rem 0 0.5rem 0;
	}
</style>
