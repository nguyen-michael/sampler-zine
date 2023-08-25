<script lang="ts">
	import { fade } from 'svelte/transition';
</script>

<div transition:fade>
	<slot />
</div>

<style>
	div {
		position: relative;

		grid-area: 1 / 1 / 2 / 2;

		width: 600px;
		height: 430px;
		border: 2px solid black;

		background-color: white;
		color: black;
	}
</style>
