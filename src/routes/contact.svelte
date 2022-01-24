<svelte:head>
	<title>Contact Me | CMF</title>
</svelte:head>

<div class="contact">
	<form action="https://formsubmit.co/chris@cmfred.com" method="post">
		<h2>
			Contact Me
			<i class="material-icons-outlined">mail</i>
		</h2>
		<label for="name">Name:</label>
		<input type="text" name="name" id="name" placeholder="Name" required />

		<label for="email">Email:</label>
		<input type="email" name="email" id="email" placeholder="Email" required />

		<label for="phone">Phone Number:</label>
		<input type="tel" name="phone" id="phone" placeholder="Phone Number" />

		<label for="message">Message:</label>
		<textarea name="message" id="message" cols="30" rows="10" />

		<input type="hidden" name="_next" value="https://cmfred-dev.netlify.app/thanks" />
		<input type="hidden" name="_captcha" value="false" />
		<input type="hidden" name="_subject" value="CM Fred Dev" />

		<button type="submit">Send</button>
	</form>
	<div class="text-box">
		<h2>Thank You for stopping by!</h2>
		<p class="top">
			Please contact me if you want to get your business online. I can help you each step of the
			way, from planning and design to development and deployment!
		</p>
		<ul>
			<li>Professional Graphic Design</li>
			<li>Custom Color Scheme</li>
			<li>Built for a Great User Experience</li>
			<li>Developed to be Fast</li>
		</ul>
		<p class="bottom">
			I will handle all of the technology so you don't have to! You can focus on your primary
			business, I will take care of your website.
		</p>

		<div class="icon-bar">
			<i class="material-icons-outlined">terminal</i>
			<i class="material-icons-outlined">store</i>
			<i class="material-icons-outlined">rocket_launch</i>
			<i class="material-icons-outlined">computer</i>
			<i class="material-icons-outlined">desktop_windows</i>
		</div>
	</div>
</div>

<style>
	.contact {
		display: flex;
	}
	form {
		display: flex;
		flex-direction: column;
		background-color: var(--clr-primary-dark-transparent);
		width: 100%;
		max-width: 600px;
		padding: 1rem 1.5rem 2rem;
		border-radius: 1rem;
		border: 2px solid var(--clr-accent);
		outline: 1px solid var(--clr-accent-pink);
	}

	h2 {
		display: flex;
		justify-content: space-between;
		align-items: center;
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
		font-family: var(--font-text);
		padding: 0.5rem;
		border-radius: 0.5rem;
		background-color: var(--clr-accent);
	}

	textarea::placeholder {
		color: var(--clr-primary-dark);
		padding-top: 0.5rem;
		font-size: 1rem;
	}

	button {
		width: 50px;
		line-height: 2;
		background-color: var(--clr-accent-pink);
		border: none;
		color: var(--clr-accent);
		font-family: var(--font-link);
		font-weight: bold;
		margin: 1rem auto;
		padding: 0 0.5rem;
		border-radius: 0.25rem;
	}

	.text-box {
		width: 50%;
		padding: 0 2rem;
	}

	.text-box h2 {
		margin-bottom: 1rem;
	}

	ul {
		list-style: none;
		margin: 1rem 2rem;
	}

	li::before {
		content: '\2745';
		color: var(--clr-accent-pink);
		margin-right: 0.25rem;
		font-weight: bold;
	}

	.icon-bar {
		text-align: center;
		background-color: var(--clr-primary-dark);
		border: 5px dotted var(--clr-accent-pink);
		opacity: 80%;
		margin: 2rem auto;
		border-radius: 0.5rem;
		padding: 0.5rem 0;
	}

	.icon-bar i {
		font-size: 3rem;
	}

	@media (max-width: 768px) {
		.contact {
			display: block;
		}

		.text-box {
			width: unset;
			padding: 0 0.25rem;
			margin-top: 2.5rem;
		}

		p {
			font-size: 1.25rem;
			padding-bottom: 2rem;
		}

		p.top {
			border-bottom: 5px solid var(--clr-accent-pink);
		}

		p.bottom {
			border-top: 5px solid var(--clr-accent-pink);
			padding-top: 2rem;
		}

		ul {
			outline: 2px solid var(--clr-accent);
			margin: 2rem 1.5rem;
			text-align: start;
			padding: 1rem 2.5rem;
		}

		li {
			margin: 0.25rem 0;
		}

		li::before {
			margin-left: -1.25rem;
		}
	}
</style>
