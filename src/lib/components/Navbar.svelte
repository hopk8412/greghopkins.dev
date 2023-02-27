<nav class="navbar">
	<div class="navbar-container">
		<a href="/" class="nav-item">Home</a>
		<a href="/about" class="nav-item">About</a>
		<a href="/portfolio" class="nav-item">Portfolio</a>
	</div>
</nav>

<style>
    @media screen and (max-width: 600px) {
  .navbar-container {
    flex-direction: column;
}
}
	.navbar {
		display: flex;
		justify-content: center;
	}
	.navbar-container {
		display: flex;
		justify-content: center;
		background-color: #291528;
		border-radius: 12px;
		box-shadow: 10px 5px 5px #5e4988;
		width: 50%;
	}
	.nav-item {
		padding: 30px;
		text-decoration: none;
		color: #fff;
	}
	.nav-item:hover {
		color: #8a4fff;
		transition: 0.3s;
	}
	@font-face {
		font-family: 'Rodin';
		src: local(''), url('/fonts/FOTRodin Pro DB.otf') format('opentype');
	}
	.nav-item {
		font-family: 'Rodin', 'Helvetica Neue', sans-serif;
	}
</style>
