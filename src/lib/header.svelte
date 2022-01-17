<script lang="ts">
	import Nav from './nav.svelte';
</script>

<header>
	<h1><a href="/">CM FREDRICKSEN Development</a></h1>
	<h2 class="icon">&#9729</h2>
	<Nav />
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		align-items: center;
		background-color: var(--clr-primary-dark);
		padding: 2rem;
	}
	h1 {
		margin: 0;
	}
	.icon {
		color: var(--clr-accent);

		font-size: 3rem;
		margin: 0;
		margin-block-start: 0;
		margin-block-end: 0;
	}
</style>
