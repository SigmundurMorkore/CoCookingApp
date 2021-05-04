<script>
	import Jitsi from '../lib/Jitsi.svelte';
</script>

<article>
	<header>
		<h1>Persian Kuku with Spinach and Wild Ramps</h1>
	</header>
	<main>
		<p>Recipe serves 10</p>
		<section>
			<h2>Ingredients</h2>
			<ul>
				<li>700 g Coarsely chopped spinach</li>
				<li>
					300 g Coarsely chopped wild ramps (alternatively use 3 garlic cloves and 1 kg spinach)
				</li>
				<li>5 Tbl spoons flour</li>
				<li>5 Eggs</li>
				<li>Salt and pepper</li>
			</ul>
		</section>
		<section>
			<h2>Instructions</h2>
			<p>
				Squeeze excess water from spinach (if bought frozen). Mix spinach wild ramps and eggs in a
				bowl and add salt and pepper. Prepare in pan with oil until golden brown and firm. Flip kuku
				omelette to cook on both sides.
			</p>
			<p>
				For a herb version of kuku add a combination of cinnamon, walnuts and blueberries or
				parsley, cilantro, dill, and scallions.
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
			url('https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.thejc.com%2Fimage%2Fpolicy%3A1.486639%3A1563457841%2FIMG-0020high-res.jpg%3Ff%3D16x9%26h%3D576%26w%3D1024%26%24p%24f%24h%24w%3D7e1b886&f=1&nofb=1');
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
