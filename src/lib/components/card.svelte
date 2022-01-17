<script>
	export let title;
	export let icon;
	export let list;
	export let link;
</script>

<div class="card">
	<h2>{title}</h2>
	<h2>&#9729;{icon}</h2>

	<ul>
		{#each list as item}
			<li>{item}</li>
		{/each}
	</ul>
	<button>{link}</button>
</div>
