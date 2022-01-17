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
		padding: 2rem 2rem 3rem;
		max-width: 90vw;
		margin: 0 auto;
	}
</style>
