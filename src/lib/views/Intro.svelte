<script lang="ts">
	import Frame from '../atoms/Frame.svelte';
	import sampler1 from '$lib/images/sampler-1.jpeg';
</script>

<Frame>
	<div>
		<h1>SAMPLER</h1>
		<h2>A funky FREE FONT</h2>
		<img alt="abc" src={sampler1} />
	</div>
</Frame>

<style>
	div {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	img {
		max-width: 30%;
		height: 30%;
	}
</style>
