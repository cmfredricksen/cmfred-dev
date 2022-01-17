<script>
	import Card from '$lib/components/card.svelte';

	export let cards = [
		{
			title: 'Creative Solutions',
			icon: '&hearts;',
			list: [
				'Professional Graphic Design',
				'Quality Websites Built for Your Business',
				'Worry Free Site Maintenance'
			],
			link: 'services'
		},
		{
			title: 'High Quality Work',
			icon: '&diams;',
			list: ['Attention to Detail', 'Search Engine Optimization', 'Website Backups and Updates'],
			link: 'contact'
		}
	];
</script>

<svelte:head>
	<title>Chris F. Dev | Home</title>
</svelte:head>
<div class="main">
	<h3>Custom Web Solutions Tailored for Your Needs!</h3>

	<p>
		You have plenty to do, let me take care of your website. I will plan, design, build, deploy and
		maintain your web presence so you can focus on running your primary business. Each website is
		custom built with attention to detail and an eye on quality. I have years of experience building
		websites using different technologies and platforms. I will handle the details so you don't have
		to.
	</p>
	<!-- <img src="/static/images/pexels-castorly-stock-4065748.jpg" alt="" /> -->
	<div class="img-div" />

	{#each cards as card}
		<Card {...card} />
		<!-- {card.title}{card.icon}{card.link} -->
	{/each}
</div>

<style>
	.main {
		max-width: 100%;
	}

	h3 {
		text-align: center;
	}

	p {
		margin: 0.5rem 0 2rem;
		line-height: 1.3;
	}

	.img-div {
		background-image: url('/static/images/pexels-castorly-stock-4065748.jpg');
		background-repeat: no-repeat;
		display: block;
		height: 150px;
		background-size: 100%;
		background-position-x: left;
		background-position-y: center;
		border-radius: 1rem;
		border: 2px solid var(--clr-primary-dark);
		outline: thick double var(--clr-accent-pink);
		margin: 0 auto 2rem;
		width: 90%;
	}
</style>
