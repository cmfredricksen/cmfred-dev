<svelte:head>
	<title>Thank You | CM Fred</title>
</svelte:head>

<div class="thank-you">
	<h1>Thank you!</h1>

	<p>Your message has been sent, I will get back to you soon.</p>

	<i class="material-icons-outlined">check_circle</i>
</div>

<style>
	.thank-you {
		display: flex;
		flex-direction: column;
		justify-content: space-around;
		align-items: center;
		height: 200px;
		margin: 1rem auto;
		/* text-align: center; */
	}

	p {
		font-size: 1.5rem;
	}

	i {
		color: var(--clr-accent-pink);
		font-size: 2rem;
	}

	@media (max-width: 768px) {
		.thank-you {
			flex: 1;
			justify-content: space-between;
			height: 100%;
		}
		p {
			text-align: center;
			line-height: 2.5rem;
			margin: 1.5rem 1rem;
		}
	}
</style>
