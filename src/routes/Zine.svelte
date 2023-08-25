<script lang="ts">
	import Acknowledgements from '$lib/views/Acknowledgements.svelte';
	import Coda from '$lib/views/Coda.svelte';
	import Intro from '$lib/views/Intro.svelte';
	import Sandbox from '$lib/views/Sandbox.svelte';
	import Story from '$lib/views/Story.svelte';

	const pages = [Intro, Story, Sandbox, Coda, Acknowledgements];
	let currentPage = pages[0];

	const cyclePages = () => {
		currentPage = pages[(pages.indexOf(currentPage) + 1) % pages.length];
	};
</script>

<div>
	<svelte:component this={currentPage} />
	<button on:click={cyclePages}>↠</button>
</div>

<style>
	div {
		display: grid;
		grid-template-rows: 3fr 1fr;
	}

	button {
		color: rgba(255, 255, 255, 0.87);
		background-color: #242424;
		font-size: 3rem;
	}
</style>
