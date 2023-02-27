<script>
	export let cardColorOptions;
	function shuffle(array) {
		let currentIndex = array.length,
			randomIndex;

		// While there remain elements to shuffle.
		while (currentIndex != 0) {
			// Pick a remaining element.
			randomIndex = Math.floor(Math.random() * currentIndex);
			currentIndex--;

			// And swap it with the current element.
			[array[currentIndex], array[randomIndex]] = [array[randomIndex], array[currentIndex]];
		}

		return array;
	}
</script>

<div class="card {shuffle(cardColorOptions).pop()}">
	<div class="card-header"><slot name="cardHeader"><h1>Default Header Text</h1></slot></div>
	<div class="card-content"><slot name="cardContent"><p>Default Card Content</p></slot></div>
</div>

<style>
	.card {
		margin: 30px;
		padding: 10px;
		text-align: center;
		border-radius: 60px;
		box-shadow: 10px 5px 5px gray;
		display: inline-block;
		justify-content: center;
		width: 400px;
		/* background-color: #087e8b; */
		transition: 0.6s;
	}

	.vermillion {
		background-color: #f24236;
	}

	.blue {
		background-color: #087e8b;
	}

	.dark-purple {
		background-color: #291528;
	}

	.light-purple {
		background-color: #8a4fff;
	}

	.card:hover, .card:active {
		transform: translate(0, -10px);
		transition: 0.6s;
	}

	.card-header,
	.card-content {
		color: #fff;
		padding: 10px;
	}

    @font-face {
		font-family: 'Lato';
		src: local(''), url('/fonts/Lato-Regular.ttf') format('truetype');
	}
	* {
		font-family: 'Lato', 'Helvetica Neue', sans-serif;
	}
</style>
