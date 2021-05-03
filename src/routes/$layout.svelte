<svelte:head>
	<style>
		@import 'https://meyerweb.com/eric/tools/css/reset/reset.css';
	</style>
</svelte:head>

<div>
	<header>
		<h1>CoCooking</h1>
	</header>

	<nav>
		<h2>Recipies</h2>
		<ul>
			<li>MEZZE MANICHE ALLA GRICIA</li>
		</ul>
	</nav>

	<main>
		<slot />
	</main>
</div>

<style>
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
