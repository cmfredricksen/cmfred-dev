<script lang="ts">
	import Card from '$lib/components/card.svelte';

	export let cards = [
		{
			title: 'Creative Solutions',
			icon: 'lightbulb',
			list: ['Professional Graphic Design', 'Custom Built for You', 'Attention to Detail'],
			link: 'services'
		},
		{
			title: 'High Quality Work',
			icon: 'diamond',
			list: [
				'Search Engine Optimization',
				'Website Backups and Updates',
				'Worry Free Site Maintenance'
			],
			link: 'contact'
		}
	];
</script>

<svelte:head>
	<title>CMF Dev | Home</title>
</svelte:head>
<div class="main">
	<h3>Custom Web Solutions Tailored for Your Needs!</h3>

	<p class="intro-text">
		You have plenty to do, let me take care of your website. I will plan, design, build, deploy and
		maintain your website so you can focus on running your primary business. Each website is custom
		built with attention to detail and an eye on quality. I will handle the details so you don't
		have to.
	</p>

	<p class="body-text">
		Having a website is a great way for your clients to find you, get in touch with you, and keep up
		with your latest work. It is also a wonderful way for you to find more clients as your website
		is available 24 hours a day, 7 days a week, holidays included! It is your piece of real estate
		on the web. It lets people know you are there, and what services and/or products you provide.
	</p>

	<div class="img-div">
		<div class="icon-bar">
			<i class="material-icons-outlined">terminal</i>
			<i class="material-icons-outlined">store</i>
			<i class="material-icons-outlined">rocket_launch</i>
			<i class="material-icons-outlined">computer</i>
			<i class="material-icons-outlined">desktop_windows</i>
		</div>
	</div>

	<p class="body-text">
		I specialize in small businesses and solo entrepeneurs who are looking for a unique, custom
		built website that reflects their core message and values. I use the best techniques to ensure
		your website will load quickly and work smoothly for your visitors, whether they are using a
		computer, a tablet or a smart phone.
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
		font-size: 1.25rem;
		font-style: oblique;
	}

	.img-div {
		background-image: url('/static/images/keyboard.jpg');
		background-repeat: no-repeat;
		display: flex;
		height: 150px;
		background-size: 100%;
		background-position-x: left;
		background-position-y: center;
		border-radius: 0.5rem;
		margin: 0 auto 2rem;
		width: 90%;
	}
	.icon-bar {
		width: 100%;
		margin: 0 auto;
		display: flex;
		align-items: center;
		justify-content: space-around;
		background-color: var(--clr-primary-dark-transparent);
		padding: 2rem 0.5rem;
		border: 1px solid var(--clr-accent);
		border-radius: 0.5rem;
	}

	.icon-bar i {
		font-size: 4rem;
	}
	.body-text {
		font-size: 1.25rem;
		margin: 2rem 0;
	}

	.card-container {
		margin: 1rem auto;
		display: flex;
		justify-content: space-evenly;
	}

	@media (max-width: 768px) {
		h3 {
			font-size: 2.5rem;
			line-height: 1;
			margin: 0 1rem;
		}

		.intro-text {
			border-bottom: 3px solid var(--clr-accent-pink);
			padding-bottom: 01.25rem;
			margin-left: 0.5rem;
		}

		.body-text {
			margin-left: 0.5rem;
		}

		.img-div {
			/* display: none; */
			width: 100%;
		}

		.card-container {
			flex-direction: column;
			justify-content: space-between;
			align-items: center;
		}
	}
</style>
