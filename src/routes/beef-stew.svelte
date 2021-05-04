<script>
	import Jitsi from '../lib/Jitsi.svelte';
</script>

<article>
	<header>
		<h1>Beef stew with cabbage and lentils</h1>
	</header>
	<main>
		<p>4 servings</p>
		<section>
			<h2>Ingredients</h2>
			<ul>
				<li>300 g ground beef</li>
				<li>2 large onions</li>
				<li>2 tbsp. oil</li>
				<li>200 g green lentils</li>
				<li>¼ head of white cabbage</li>
				<li>1 tsp. dried rosemary</li>
				<li>Water or stock</li>
				<li>Salt and pepper</li>
				<li>Garnish with wild herbs e.g. Chervil</li>
			</ul>
		</section>
		<section>
			<h2>Instructions</h2>
			<p>
				Chop onions coarsely and heat in pan with oil until clear/transparent. Add meat and continue
				cooking until meat is finished. Add lentils, chunks of coarsely cut cabbage, rosemary and
				salt. Cover with water or stock and cook until lentils are tender. Add salt, pepper and
				rosemary to taste. Serve with freshly chopped garnish e.g. wild Chervil.
			</p>
		</section>
	</main>

	<Jitsi roomName="CoCooking-persian-kuku" />
</article>

<style>
	main {
		padding: 10px;
	}

	section {
		padding-top: 1rem;
	}
	section h2 {
		font-family: Montserrat;
		font-style: normal;
		font-weight: bold;
		font-size: 24px;
		line-height: 29px;
		display: flex;
		align-items: center;
	}
	ol {
		padding-left: 30px;
		list-style: decimal;
	}
	li {
		font-size: 18px;
		line-height: 163.9%;
	}

	article {
		width: 100%;
		display: grid;
		grid-gap: 1rem;
		grid-template-areas:
			'header header'
			'instructions jitsi ';
	}

	header {
		grid-area: header;
		display: flex;
		align-items: center;
		justify-content: center;

		height: 350px;
		width: 100%;

		background: linear-gradient(0deg, rgba(255, 255, 255, 0.5), rgba(255, 255, 255, 0.5)),
			url('https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fthefirstmess.com%2Fwp-content%2Fuploads%2F2019%2F12%2F31-11889-post%2Fsmoky-chickpea-cabbage-lentil-stew-kale-vegan-recipe-7.jpg&f=1&nofb=1');
		box-shadow: inset 0px -130px 100px #ffffff;
		background-size: cover;
		background-position: center;
	}
	header h1 {
		font-family: Montserrat;
		font-style: normal;
		font-weight: bold;
		font-size: 48px;
		line-height: 59px;
		display: flex;
		align-items: center;
		text-align: center;
	}
</style>
