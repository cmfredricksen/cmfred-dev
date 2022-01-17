<script lang="ts">
	import Nav from './nav.svelte';
	const sayHello = () => {
		console.log('Hello');
	};
</script>

<header>
	<h2><a href="/">CM FREDRICKSEN Development</a></h2>
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
</style>
