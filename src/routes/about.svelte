<script lang="ts">
	import Album from '$lib/components/album.svelte';
</script>

<svelte:head>
	<title>About Me | CMF</title>
</svelte:head>

<h2>About Me</h2>
<div class="about">
	<h3 class="about title">I am a Creative Problem Solver with an Eye for Design</h3>

	<p>
		I am a developer, a designer and an artist with a passion for creating web pages that are
		beautiful and easy to use. I get real satisfaction with each project that I finish, combining
		technology with visual art to build clean designs with eye-popping color.
	</p>

	<p>
		My first computer programming was in the early 1980's when I was a kid. When I grew up I got my
		A.S. Degree in Graphic Design and have since worked as a graphic designer, web developer and
		fine artist amongst other things.
	</p>

	<p>
		I love creativity of all types, from literature to sculpture, painting to photography, animation
		to movies. It is inspiring. It is interesting to see the expression of different people, how
		they are different and yet the same.
	</p>

	<Album />

	<p>
		Cooking is another creative outlet, I cook dinner most nights for myself and my kids. I enjoy
		trying new recipes and just making recipes up based on my cooking experience.
	</p>

	<p>
		I am always learning new things and studying new topics. My most visited website is the <a
			href="https://www.noaa.gov/">NOAA</a
		>
		and
		<a href="https://www.weather.gov">NWS</a> because it is a never ending source of interesting data.
		I also appreciate how well they incorporate all of that data into a fairly easy to navigate website.
		It is truly impressive!
	</p>

	<p>
		I have an eye for detail and I am very conscientious about my work. I am very focused when I am
		planning and building a project. I know how to find the answers I need as challenges arise. I
		will get the job done and I will do it well!
	</p>

	<div class="hobby-container">
		<img src="/static/images/forest.jpg" alt="Forest" title="Tranquil Morning" />

		<ul class="hobby-list">
			Other Hobbies:
			<li>Birding</li>
			<li>Hiking</li>
			<li>Tai CHi</li>
			<li>Reading</li>
			<li>Geography</li>
			<li>History</li>
			<li>Diarist</li>
			<li>Movies & Series</li>
		</ul>

		<div class="thank-you">
			<p>Thank you for visiting!</p>
			<a href="mailto:chris@cmfred.com&subject=Website%20Inquiry">Contact Me</a>
		</div>
	</div>
</div>

<style>
	h2 {
		color: var(--clr-accent-pink);
		text-align: center;
	}
	h3 {
		color: var(--clr-accent);
		margin: 0.5rem 1.5rem;
	}
	div {
		padding: 1rem 0 2rem;
		margin-top: 1.5rem;
	}
	.about {
		background: var(--clr-primary-dark);
		border-radius: 0.5rem;
	}
	p {
		margin: 0.5rem 1.5rem;
		line-height: 1.4;
		font-size: 1.25rem;
	}

	a {
		margin: 0.5rem 0;
	}

	.hobby-container {
		display: grid;
		grid-template-columns: 1.5fr 0.5fr 1.5fr;
	}

	img {
		margin: 0 auto;
		border-left: 3px solid var(--clr-accent-pink);
	}

	ul {
		list-style: none;
		color: var(--clr-accent-pink);
		text-align: center;
	}

	li {
		color: var(--clr-accent);
	}

	.thank-you {
		display: flex;
		flex-direction: column;
		margin: 0 auto;
		padding: 0 3rem;
		border: 3px dashed var(--clr-accent-pink);
		border-radius: 0.55555rem;
		align-items: center;
		justify-content: center;
	}

	.thank-you p {
		margin: 0;
	}
</style>
