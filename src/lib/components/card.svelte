<script lang="ts">
	export let title: string;
	export let icon: string;
	export let list: string[];
	export let link: string;
</script>

<div class="card">
	<h2>{title}</h2>
	<h1 class="card-icon"><i class="material-icons-outlined">{icon}</i></h1>

	<ul>
		{#each list as item}
			<li>
				<!-- <p>{icon}</p> -->
				<p><i class="material-icons-outlined">{icon}</i>{item}</p>
				<!-- {item} -->
			</li>
		{/each}
	</ul>
	<a class="link-button" href="/{link}">{link}</a>
</div>

<style>
	.card {
		border: 0.25rem solid var(--clr-accent);
		padding: 2rem 2rem 1rem;
		border-radius: 1rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		width: 30vw;
		margin: 0 2rem;
		background-color: var(--clr-primary-dark);
		box-shadow: 2px 2px 3px black;
	}

	h1 {
		background-color: var(--clr-accent-pink);
		color: var(--clr-text);
		opacity: 80%;
		text-shadow: 1px 1px 1px var(--clr-primary-dark);
		border: 2px solid var(--clr-accent);
		border-radius: 0.25rem;
		font-size: 3rem;
		margin: 1.5rem auto 1rem;
		width: 20%;
		padding: 1rem 0.25rem 0;
	}

	.card-icon {
		width: 5rem;
	}

	h1,
	h2,
	ul {
		text-align: center;
	}

	li {
		display: flex;
		align-items: center;
		justify-content: baseline;
		list-style: none;
		/* line-height: 2rem; */
	}

	li > p {
		margin: 0.5rem;
		color: var(--clr-accent);
	}

	p i {
		color: var(--clr-accent-pink);
		margin-right: 0.25rem;
		font-size: 0.85rem;
	}

	.link-button {
		margin: 2.5rem auto 1rem;
		padding: 0.35rem 0.5rem;
		border: 0.1rem solid var(--clr-text);
		outline: 0.2rem solid var(--clr-accent-pink);
		font-weight: bold;
		border-radius: 0.5rem;
		background-color: var(--clr-accent);
		color: var(--clr-primary-dark);
	}

	.link-button:hover {
		color: var(--clr-accent-pink);
		background-color: var(--clr-primary-dark);
	}
</style>
