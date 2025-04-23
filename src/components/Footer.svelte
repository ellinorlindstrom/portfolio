<script>
	const currentYear = new Date().getFullYear();
</script>

<footer>
	<section class="social-icons">
		<img src="../icons/mail.png" alt="mail icon" width="30" height="30" loading="lazy" />
		<img src="../icons/github.png" alt="github icon" width="30" height="30" loading="lazy" />
		<img src="../icons/linkedin.png" alt="linkedin icon" width="30" height="30" loading="lazy" />
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
