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
			<li>{item}</li>
		{/each}
	</ul>
	<button>{link}</button>
</div>
