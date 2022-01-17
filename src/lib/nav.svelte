<script lang="ts">
	const links = [
		{
			name: 'Home',
			href: '/'
		},
		{
			name: 'About',
			href: '/about'
		},
		{
			name: 'WebFolio',
			href: 'https://webfolio-cmfredricksen.netlify.app'
		},
		{
			name: 'Services',
			href: '/services'
		},
		{
			name: 'Contact',
			href: '/contact'
		}
	];
</script>

<nav>
	{#each links as link}
		<a href={link.href}>{link.name}</a>
	{/each}
</nav>

<style>
	a {
		margin: 0 0.5rem;
	}
</style>
