<script>
	import { page } from '$app/stores';
	const links = [
		{
			name: 'Home',
			path: '/'
		},
		{
			name: 'About',
			path: '/about'
		},
		{
			name: 'WebFolio',
			path: 'https://webfolio-cmfredricksen.netlify.app',
			target: '_blank'
		},
		{
			name: 'Services',
			path: '/services'
		},
		{
			name: 'Contact',
			path: '/contact'
		}
	];
</script>

<nav>
	{#each links as link}
		<a
			class:active={// @ts-ignore
			$page.url.pathname === link.path}
			href={link.path}
			target={link.target}>{link.name}</a
		>
	{/each}
</nav>

<style>
	a {
		margin: 0 0.5rem;
	}

	.active {
		text-decoration: underline var(--clr-accent-pink);
	}
</style>
