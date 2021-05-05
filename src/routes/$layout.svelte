<svelte:head>
	<style>
		@import 'https://meyerweb.com/eric/tools/css/reset/reset.css';
		@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');
	</style>
</svelte:head>

<div>
	<header>
		<h1>CoCooking App</h1>
	</header>

	<nav>
		<h2>Recipies:</h2>
		<ul>
			<li><a href="mezze">Mezze Maniche Alla Gricia</a></li>
			<li><a href="beef-stew">Beef Stew</a></li>
			<li><a href="rosehip">Rosehip Marmalde</a></li>
			<li><a href="persian-kuku">Persian Kuku</a></li>
			<li><a href="pakistani-vegetable">Pakistani Vegetable Curry</a></li>
		</ul>
	</nav>

	<main>
		<slot />
	</main>
</div>

<style>
	a {
		color: inherit;
		text-decoration: none;
	}
	li {
		margin-left: 20px;
		padding-top: 10px;
	}

	div {
		display: grid;
		grid-template-areas:
			'header header header'
			'nav main main';
	}
	header {
		grid-area: header;

		background-color: #bfc78a;
		height: 70px;
		font-family: Montserrat;
		font-style: normal;
		font-weight: bold;
		font-size: 36px;
		line-height: 44px;
	}
	h1 {
		margin-top: 10px;
		margin-left: 1rem;
	}

	nav {
		grid-area: nav;

		min-height: 100vh;
		background: #412516;
		color: white;

		padding: 10px;
	}
	nav h2 {
		font-family: Montserrat;
		font-style: normal;
		font-weight: normal;
		font-size: 24px;
		line-height: 29px;
	}

	main {
		grid-area: main;
		width: 1fr;
	}
</style>
