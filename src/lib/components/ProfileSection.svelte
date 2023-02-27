<div class="profile-section">
        <img class="profile-image" src="/images/black_mage_ff.png" alt="Me" height="150" width="150" />
		<h2 class="profile-header">Greg Hopkins</h2>
        <p class="info">Software Engineer since 5/2020</p>
        <figure class="quote">
            <blockquote>
                "You have power over your mind &mdash; not outside events. Realize this, and you will find strength."
            </blockquote>
            <figcaption>
                &mdash; Marcus Aurelius, <cite>Meditations</cite>
            </figcaption>
        </figure>
</div>

<style>
    @media screen and (max-width: 600px) {
  .profile-section {
    align-self: center;
    width: 50%;
    flex-shrink: 2;
}
}
	.profile-section {
		background-color: #087e8b;
        box-shadow: 10px 5px 5px gray;
		color: #fff;
		border-radius: 30px;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
	}

    .profile-header {
        margin: 0;
    }

	.profile-image {
        justify-self: center;
        align-self: center;
		border: 5px solid black;
		border-radius: 300px;
		margin: 20px;
	}
    .info {
        text-align: center;
        margin-bottom: 0;
    }
    .quote {
        margin-top: 0;
        display: inline-block;
        text-align: center;
        width: 100%;
        max-width: 200px;
    }

	@font-face {
		font-family: 'Lato';
		src: local(''), url('/fonts/Lato-Regular.ttf') format('truetype');
	}
	* {
		font-family: 'Lato', 'Helvetica Neue', sans-serif;
	}
</style>
