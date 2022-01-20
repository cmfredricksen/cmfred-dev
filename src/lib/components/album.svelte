<script lang="ts">
	let images = [
		{ name: 'Chickadee', path: '/static/images/chickadee.jpg' },
		{ name: 'Cooking', path: '/static/images/cooking.jpg' },
		{ name: 'Movies', path: '/static/images/movies.jpg' }
	];
</script>

<div class="album">
	<div class="container">
		{#each images as img}
			<img src={img.path} alt={img.name} class="album-img" />
		{/each}
	</div>
</div>

<style>
	.album {
		width: 100%;
		margin: 2rem 0;
	}
	.container {
		margin: 1rem;
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;
		gap: 1rem;
	}
	.album-img {
		max-width: 100%;
		height: auto;
	}
</style>
