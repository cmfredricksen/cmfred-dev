<script lang="ts">
	import Card from '$lib/components/card.svelte';

	export let cards = [
		{
			title: 'Creative Solutions',
			icon: '♥',
			list: ['Professional Graphic Design', 'Custom Built for You', 'Worry Free Site Maintenance'],
			link: 'services'
		},
		{
			title: 'High Quality Work',
			icon: '♦',
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

	<p class="intro-text">
		You have plenty to do, let me take care of your website. I will plan, design, build, deploy and
		maintain your website so you can focus on running your primary business. Each website is custom
		built with attention to detail and an eye on quality. I have years of experience building
		websites using different technologies and platforms. I will handle the details so you don't have
		to.
	</p>
	<div class="img-div" />
	<p class="body-text">
		Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eum non voluptate adipisci maiores
		officiis voluptas tempore pariatur voluptates, alias libero aspernatur necessitatibus? Quidem,
		aliquam! Totam voluptates repudiandae eos nulla. Accusantium excepturi molestiae nisi odit,
		dolorum quae explicabo, qui omnis impedit sint ab sunt placeat suscipit itaque. Adipisci quo
		totam nihil deleniti repellendus inventore provident veniam asperiores! Nesciunt, reprehenderit
		laborum praesentium temporibus, mollitia velit voluptas magnam a, dolorum aliquid id ipsum
		pariatur natus illo totam blanditiis veritatis sequi dignissimos atque fuga? Quas autem ipsum ut
		eaque voluptas blanditiis quibusdam temporibus, tempore, nobis, quisquam reprehenderit! Suscipit
		eos harum, error aspernatur minima cumque.
	</p>

	<div class="card-container">
		{#each cards as card}
			<Card {...card} />
		{/each}
	</div>
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

	.intro-text {
		font-size: 1.5rem;
		font-style: oblique;
	}
	.body-text {
		columns: 2;
		column-gap: 2rem;
		text-align: justify;
		font-size: 1.25rem;
		margin: 2rem 0;
		padding: 2rem 0;
	}

	.img-div {
		background: linear-gradient(
				var(--clr-primary-dark-transparent-33),
				var(--clr-primary-dark-transparent-33)
			),
			url('/static/images/pexels-castorly-stock-4065748.jpg');
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

	.card-container {
		margin: 1rem auto;
		display: flex;
		justify-content: space-evenly;
	}
</style>
