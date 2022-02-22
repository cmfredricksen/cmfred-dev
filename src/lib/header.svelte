<script lang="ts">
	import Nav from './nav.svelte';
	const sayHello = () => {
		console.log('Hello');
	};
</script>

<header>
	<a href="#wrapper" class="skip-nav-link">skip navigation</a>
	<h2 class="title"><a href="/">CM FREDRICKSEN Development</a></h2>
	<h2 class="icon" on:click={sayHello}>&#10053</h2>
	<Nav />
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		align-items: center;
		background-color: var(--clr-primary-dark);
		padding: 1rem;
	}

	.skip-nav-link {
		position: absolute;
		transform: translateY(-320%);
		translate: transform 325ms ease-in;
	}

	.skip-nav-link:focus {
		transform: translateY(-170%);
	}

	h2 {
		margin: 0;
	}

	.icon {
		background-color: var(--clr-accent-pink);
		color: var(--clr-text);
		opacity: 80%;
		text-shadow: 1px 1px 1px var(--clr-primary-dark);
		border: 2px solid var(--clr-accent);
		border-radius: 3rem;
		font-size: 3rem;
		margin: 0.3rem;
		padding: 0 0.75rem;
	}

	.icon:hover {
		background-color: var(--clr-accent);
		color: var(--clr-primary-dark);
		opacity: 100%;
		text-shadow: 1px 1px 1px var(--clr-accent-pink);
		border: 2px solid var(--clr-accent-pink);
	}

	@media (max-width: 768px) {
		header {
			display: block;
			padding: 1rem 0;
			position: sticky;
			top: 0;
		}

		.title {
			text-align: center;
		}

		h2.icon {
			text-align: center;
			padding: 0.25rem 0;
			font-size: 1rem;
			border-radius: 0;
			margin: 1.5rem 0;
		}
	}
</style>
