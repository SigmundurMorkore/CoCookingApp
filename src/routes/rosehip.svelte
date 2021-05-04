<script>
	import Jitsi from '../lib/Jitsi.svelte';
</script>

<article>
	<header>
		<h1>Rosehip Marmalade</h1>
	</header>
	<main>
		<section>
			<h2>Ingredients</h2>
			<ul>
				<li>2 kg cleaned hibs</li>
				<li>½ liter water</li>
				<li>600 grams honey</li>
				<li>4 lemons</li>
				<li>2 vanilla roots</li>
				<li>Atamon</li>
			</ul>
		</section>
		<section>
			<h2>Instructions</h2>
			<p>
				Remove flower and stem then cut rosehip in half. Scrape out the seeds and rinse thoroughly.
				Wash lemons and grate for lemon rinds. Cook cleaned rosehips in water and without lid for 20
				min. Add juice of 2 lemons, lemon rinds and a split vanilla fruit to water while cooking.
				Add honey and let simmer for another 15 minutes.
			</p>
			<p>
				Rinse canning jars and lids in boiling water (add 1 tbl. Atamon to water). To preserve your
				rosehip marmalade add 1 tsp. Atamon to each glass.
			</p>
			<p>Recipe makes 7+ jars depending on size</p>
		</section>
	</main>

	<Jitsi roomName="CoCooking-rosehip" />
</article>

<style>
	p {
		padding-top: 1rem;
	}

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
			url('https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2F3.bp.blogspot.com%2F-S90CnURSQUk%2FTlR7Yuc1cKI%2FAAAAAAAADOk%2FkE4C8E6BTsA%2Fs1600%2Frh1.jpg&f=1&nofb=1');
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
