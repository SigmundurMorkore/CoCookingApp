<script>
	// Set the default value for roomName to be "CoCooking"
	export let roomName = 'CoCooking';

	import { onMount } from 'svelte';

	// Set the initial variables
	let jitsiReady = false;
	let jitsiHasLoaded = false;
	let mounted = false;

	let api;

	// When component mounts:
	onMount(() => {
		mounted = true;
	});

	// When Jitsi has loaded:
	function jitsiLoaded() {
		// The external Jitsi javascript is ready.
		jitsiReady = true;
	}

	// Start Jitsi. Checks that the component is mounted and Jitsi is ready,
	// and if they are, it calls the loadJitsiElements() function.
	function startJitsi() {
		if (mounted && jitsiReady) {
			loadJitsiElements();
		}
	}

	// Unload Jitsi:
	function unloadJitsi() {
		api.dispose();
		jitsiHasLoaded = false;
	}

	function loadJitsiElements() {
		// Set the domain name of the Jitsi instance
		const domain = 'meet.jit.si';

		// Set the options
		const options = {
			roomName,
			width: 700,
			height: 400,
			parentNode: document.querySelector('#meet')
		};

		// Create the Jitsi element, which will attach itself to #meet
		api = new JitsiMeetExternalAPI(domain, options);

		// Indicate that Jitsi has loaded
		jitsiHasLoaded = true;

		// Listen for when the user leaves the call, and then unload Jitsi.
		api.addListener('videoConferenceLeft', unloadJitsi);
	}
</script>

<svelte:head>
	<script src="https://meet.jit.si/external_api.js" on:load={jitsiLoaded}></script>
</svelte:head>

<div>
	{#if !jitsiHasLoaded}
		<section class="jitsi">
			<h2>Join others who are cooking this recipie!</h2>
			<button on:click={() => startJitsi()}>Join video chat</button>
		</section>
	{/if}
	<div id="meet" />
</div>

<style>
	#meet {
		position: sticky;
		margin-right: 2rem;

		top: 2rem;
		height: 400px;
	}

	.jitsi {
		position: sticky;
		top: 2rem;
		width: 700px;
		height: 400px;
		background: #bfc78a;
		padding: 2rem;
		margin: 2rem;
	}
	h2 {
		font-family: Montserrat;
		font-style: normal;
		font-weight: 500;
		font-size: 36px;
		line-height: 44px;
	}
	button {
		margin-top: 40px;

		background-color: #2f5fb9;
		width: 100%;
		height: 50px;
		color: white;

		font-family: Montserrat;
		font-style: normal;
		font-weight: 500;
		font-size: 24px;
		line-height: 29px;
	}

	button:hover {
		cursor: pointer;
	}
</style>
