<script>
	import Jitsi from '../lib/Jitsi.svelte';
</script>

<article>
	<header>
		<h1>Pakistani Vegetable Curry with Wild Ramp Garnish and Green Pea Palo Rice</h1>
	</header>
	<main class="instructions">
		<section>
			<h2>Mixed vegetable curry ingredients:</h2>
			<section>
				<h3>Vegetables:</h3>
				<ul>
					<li>3 Tomatoes sliced.</li>
					<li>1 Onion Chopped.</li>
					<li>1 Cauliflower Chopped.</li>
					<li>1 Broccoli Chopped.</li>
					<li>½ kilo Peas pleaded.</li>
					<li>½ kilo Carrots Chopped.</li>
					<li>½ kilo Potatoes Diced.</li>
				</ul>
			</section>

			<section>
				<h3>Oil:</h3>
				<ul>
					<li>Ghee (clarified butter) or canola oil.</li>
					<li>Little less than ½ a cup.</li>
				</ul>
			</section>

			<section>
				<h3>Masala:</h3>
				<ul>
					<li>1 Tablespoon of Ginger & Garlic paste.</li>
					<li>½ Teaspoon Red Chilli Powder.</li>
					<li>½ Teaspoon Garam Masala.</li>
					<li>½ Teaspoon Coriander powder</li>
					<li>½ Teaspoon Turmeric</li>
					<li>Salt to taste.</li>
				</ul>
			</section>

			<section>
				<h3>Garnish:</h3>
				<ul>
					<li>Chopped wild ramps.</li>
				</ul>
			</section>
			<section>
				<h3>Method Of Cooking:</h3>
				<p>
					Add oil to hot pot after 30 seconds add chopped onion. Let the onion sweat. Then add
					garlic & ginger paste and stir for 2 minutes till paste turns light brown. Add all garam
					masala and salt cook for 1 minute on low heat. Once the masala turns RED add tomatoes and
					cook till tomatoes are dissolved and your curry is formed. Then add vegetables and stir
					for 2 minutes. Once the vegetables are covered well in the curry add ½ cup water and cover
					and cook for 35 to 45 minutes till potatoes turn tender.
				</p>
			</section>

			<section>
				<h3>Garnish:</h3>
				<p>
					Once cooked you can add chopped fresh ramps to taste. Serve with hot Pakistani green pea
					palo.
				</p>
			</section>
		</section>

		<section>
			<h2>Green Pea Palo Ingredients:</h2>
			<ul>
				<li>3 cups of rice</li>
				<li>1 cup green peas</li>
				<li>1 large onion sliced</li>
				<li>1 tablespoon garam masala</li>
				<li>1 teaspoon coriander powder</li>
				<li>5 black cardamom pods</li>
				<li>1 medium size cinnamon stick</li>
				<li>2 cubes of chicken stock</li>
				<li>Oil as needed</li>
				<li>Salt to taste</li>
			</ul>

			<section>
				<h3>Method of Cooking:</h3>
				<p>
					Add little more than half a cup of oil in pot and heat well. Add garam masala. Cook till
					you get the aroma of the masala. Add diced onion and cook until soft Add salt, chicken
					stock cubes, green peas and stir for 2 min. Add rice and stir an additional 2 mins. Add
					water just about an inch above the rice and stir well for a couple of seconds for good
					mix. Take a normal plastic bag and wrap it over the cover properly so no steam escapes.
					Once the rice comes to boil cover the pot and put something heavy on top and lower the
					heat and let cook for about 45 minutes. Add herbs when finished cooking.
				</p>
			</section>
		</section>
	</main>

	<Jitsi roomName="CoCooking-pakistani-vegetable" />
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
			url('https://www.startpage.com/av/proxy-image?piurl=https%3A%2F%2Ftheantidotekitchen.com%2Fwp-content%2Fuploads%2F2017%2F07%2FIMG_9219.jpg&sp=1620106803T1140c3b4ba5a13647a934f3eee72bca597a14e8064f842fa7eb6ac45a43ca481');
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
