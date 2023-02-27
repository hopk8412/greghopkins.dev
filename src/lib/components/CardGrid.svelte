<script>
	import Card from './Card.svelte';

	const cardColorOptions = ['vermillion', 'dark-purple', 'light-purple'];
</script>

<section id="card-grid">
	<Card {cardColorOptions}>
		<h1 slot="cardHeader">Lifelong Learner</h1>
		<p slot="cardContent">
			Something that I enjoy is learning something new. Whether it's in my sparetime or on the job, I know that I will always have room for improvement.
            To that end, I try to learn the latest in web development in terms of languages, frameworks, design patterns, and more.
		</p>
	</Card>
	<Card {cardColorOptions}>
		<h1 slot="cardHeader">My Skills</h1>
		<ul class="skillList" slot="cardContent">
			<li>Spring Boot</li>
			<li>Node.js</li>
			<li>Go</li>
		</ul>
	</Card>
	<Card {cardColorOptions}>
		<h1 slot="cardHeader">Updated Header Text</h1>
		<p slot="cardContent">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum tempore sit dolores
			architecto dignissimos autem impedit, quibusdam soluta, eos modi minima cupiditate cum
			corrupti debitis quam id aperiam beatae molestiae.
		</p>
	</Card>
</section>

<style>
	section {
		width: 100%;
		margin: 30px 0px;
		/* display: grid;
    justify-items: center;
    grid-template-columns: 1fr;
    grid-gap: 1rem; */
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}

	.skillList {
		list-style-type: '\2713\0020';
	}
</style>
