<script lang="ts">
	let images = [
		{ name: 'Chickadee', path: '/images/chickadee.jpg', title: 'chicka chickadeedeedeeee' },
		{
			name: 'Cooking',
			path: '/images/cooking.jpg',
			title: 'Some of my favorite basic ingredients'
		},
		{ name: 'Movies', path: '/images/movies.jpg', title: "It's movie night!" }
	];
</script>

<div class="album">
	<div class="container">
		{#each images as img}
			<img src={img.path} alt={img.name} class="album-img" title={img.title} />
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
