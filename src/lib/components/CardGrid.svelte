<script>
	import Card from './Card.svelte';

	const cardColorOptions = ['vermillion', 'dark-purple', 'light-purple'];
</script>

<section id="card-grid">
	<Card {cardColorOptions}>
		<h1 class="header" slot="cardHeader">My Personal Philosophy</h1>
		<p class="content" slot="cardContent">
			I am big on self-improvement and continuing education. Whether it is in my sparetime or on the job, I know that there will always be opportunities to learn more.
            To that end, I am always trying to learn new things, whether that is programming-related, new recipes, and more!
		</p>
	</Card>
	<Card {cardColorOptions}>
		<h1 class="header" slot="cardHeader">My Skills</h1>
        <div class="content" slot="cardContent">
		<p>I am a backend developer first and foremost, though I do try to keep up to date on the latest in the frontend world.</p>
        <p>Backend languages I am comfortable with include
            Java (Spring Boot), Javascript (Node.js), and Go
        </p>
        <p><strong>Note!</strong> Please view my <a class="link" href="/about">About</a> section to see a comprehensive list of my qualifications.</p>
    </div>
	</Card>
	<Card {cardColorOptions}>
		<h1 class="header" slot="cardHeader">Non-computer hobbies</h1>
		<div class="content" slot="cardContent">
			<ul class="hobbies">
                <li>Music</li>
                <li>Baking and Cooking</li>
                <li>Video Games</li>
            </ul>
        </div>
	</Card>
</section>

<style>
	section {
		width: 100%;
		margin: 30px 0px;
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
	}

	.hobbies {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        gap: 2rem;
		list-style-type: '\2713\0020';
	}

    .hobbies > li {
        flex-grow: 1;
    }
    .link {
		color: #fff;
    }

    .header {
        margin-bottom: 0;
    }
    .content {
        margin-top: 0;
    }
</style>
