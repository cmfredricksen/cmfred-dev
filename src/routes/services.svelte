<script lang="ts">
	import '../app.css';
</script>

<svelte:head>
	<title>Services Offered | CMF</title>
</svelte:head>
<div class="services">
	<h2>Services Offered</h2>

	<ul class="services-list">
		<li>Web Design</li>
		<p class="li-details">
			With a background in graphic design, web design and fine art I have an eye for colors, fonts,
			layout and the use of graphics to make beautiful web pages.
		</p>
		<li>Website Development</li>
		<p class="li-details">
			I have the know how to develop your website using everything from platforms like WordPress to
			building from scratch. Good peformance is high priority as I plan and develop your site's
			infrastructure.
		</p>
		<li>Website Deployment</li>
		<p class="li-details">
			There are many different ways to make your website go live on the web. Which you use depends
			on the type of website you have.
		</p>
		<li>Website Maintenance</li>
		<p class="li-details">
			The Web is an ever-evolving technology and sometimes you have to adjust the code so it works
			properly.
		</p>
		<li>Website Updates & Backups</li>
		<p class="li-details">
			All websites will have a backup, either using a plugin on your chosen platform or in a code
			repository if your website is hand coded. If you are using a platform, they have to be updated
			from time to time to avoid a buggy user experience.
		</p>
		<li>SEO & Analytics</li>
		<p class="li-details">
			All websites are built with Search Engine Optimization in mind, and Google Analytics to keep
			track of your traffic and user engagement.
		</p>
		<h3>and much much more!</h3>
	</ul>
</div>

<style>
	h2 {
		text-align: center;
		color: var(--clr-accent);
	}
	ul {
		list-style: none;
		padding: 2rem 1.5rem;
		margin: 2rem 0;
		border-radius: 0.5rem;
		background: var(--clr-primary-dark);
	}
	li {
		color: var(--clr-accent);
	}

	li::before {
		content: '\2745';
		color: var(--clr-text);
		padding-right: 0.5rem;
		font-size: 1.5rem;
	}
	p.li-details {
		color: var(--clr-text);
		margin: 1.5rem 1rem 1rem;
	}
</style>
