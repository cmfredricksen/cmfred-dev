<script lang="ts">
	export let title: string;
	export let icon: string;
	export let list: string[];
	export let link: string;
</script>

<div class="card">
	<h2>{title}</h2>
	<h1>{icon}</h1>

	<ul>
		{#each list as item}
			<li>
				<p>{icon}</p>
				{item}
			</li>
		{/each}
	</ul>
	<a class="link-button" href="/{link}">{link}</a>
</div>

<style>
	.card {
		border: 0.25rem solid var(--clr-accent);
		outline: 0.25rem solid var(--clr-accent-pink);
		padding: 2rem 1rem 1rem;
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
		margin: 0.5rem auto 1.5rem;
		/* padding: 0.35rem 1rem; */
		width: 20%;
	}

	h1,
	h2,
	ul {
		text-align: center;
	}

	li {
		display: flex;
		align-items: baseline;
		justify-content: center;
		list-style: none;
		line-height: 2rem;
	}

	li > p {
		margin: 0.5rem;
		color: var(--clr-accent-pink);
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
