<script lang="ts">
	import '../app.css';
	import Header from '$lib/header.svelte';
	import Footer from '$lib/footer.svelte';
</script>

<Header />

<div class="wrapper">
	<slot />
</div>

<Footer />

<style>
	.wrapper {
		background-color: var(--clr-primary-dark-transparent);
		padding: 2rem 2rem 4rem;
		max-width: 90vw;
		margin: 0 auto;
	}

	@media (max-width: 768px) {
		.wrapper {
			padding: 1.5rem 0.5rem 2.5rem;
			width: 100%;
			max-width: 100vw;
		}
	}
</style>
