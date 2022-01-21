<svelte:head>
	<title>Contact Me | CMF</title>
</svelte:head>

<div class="contact">
	<form action="" method="post">
		<h2>Contact Me</h2>
		<label for="name">Name:</label>
		<input type="text" name="name" id="name" placeholder="Name" required />

		<label for="email">Email:</label>
		<input type="email" name="email" id="email" placeholder="Email" required />

		<label for="phone">Phone Number:</label>
		<input type="tel" name="phone" id="phone" placeholder="Phone Number" />

		<label for="message">Message:</label>
		<textarea
			name="message"
			id="message"
			cols="30"
			rows="10"
			placeholder="Send me a message, I will respond as soon as possible."
		/>
	</form>
	<div class="graphic">
		<i class="material-icons-outlined">home</i>
		<i class="material-icons-outlined">mail</i>
		<i class="material-icons-outlined">favorite</i>
		<i class="material-icons-outlined">public</i>
		<i class="material-icons-outlined">face</i>
		<i class="material-icons-outlined">thumb_up</i>
	</div>
</div>

<style>
	.contact {
		display: flex;
		/* justify-content: space-between; */
	}
	form {
		display: flex;
		flex-direction: column;
		background-color: var(--clr-primary-dark-transparent);
		width: 100%;
		/* align-items: center; */
		padding: 1rem 1.5rem 2rem;
		/* justify-content: center; */
		border-radius: 1rem;
		border: 2px solid var(--clr-accent);
		outline: 1px solid var(--clr-accent-pink);
		/* margin: 1rem 0; */
	}

	label {
		font-family: var(--font-link);
		font-size: 1.25rem;
		margin-top: 1rem;
		margin-left: 0.25rem;
		margin: 1.2rem 0.25rem 0.5rem;
	}

	input {
		color: green;
		width: 70%;
		height: 2.25rem;
		border-radius: 0.5rem;
		background-color: var(--clr-accent);
		font-style: var(--clr-accent-pink);
		padding-left: 0.5rem;
	}
	input::placeholder {
		color: var(--clr-primary-dark);
	}

	textarea {
		padding-left: 0.5rem;
		border-radius: 0.5rem;
		background-color: var(--clr-accent);
	}

	textarea::placeholder {
		color: var(--clr-primary-dark);
		padding-top: 0.5rem;
		font-size: 1rem;
	}

	.graphic {
		width: 50%;
	}
</style>
