<script lang="ts">
	import Frame from '../atoms/Frame.svelte';
</script>

<Frame>
	<div>
		<section>
			<h1>TEND</h1>
			<h1>ADORE</h1>
			<h1>BLOSSOM</h1>
			<p>
				Flowers are solitary, bisexual, radial, with a long pedicel and usually floating or raised
				about the surface of the water, with girdling bundles in receptacle.
			</p>
			<p class="flowers">☙☙☙☙☙☙☙☙☙❦❧❧❧❧❧❧❧❧</p>
			<small
				>Text from the Wikipedia page on <a href="https://en.wikipedia.org/wiki/Nymphaeaceae"
					>Nymphaeaceae</a
				></small
			>
		</section>
		<section class="left">
			Sampler is a free font that contains three different weights, Regular, Bold, and Light. There
			are some symbols and glyphs missing here and there and the technical parts of a font are all
			over the place, but that is okay. I want to get better at sharing things even though they are
			not entirely done! My hope is that Sampler could be used by anyone for something sweet or fun
			that you are excited to share with the world.
			<br />
			<span>
				u can download me for free! at <a href="https://nicolettedolan.com/Sampler-2"
					>nicolettedolan.com/Sampler-2</a
				>
			</span>
		</section>
	</div>
</Frame>

<style>
	div {
		display: flex;
		flex-direction: row;

		overflow-y: scroll;
	}

	section {
		flex: 1;
		/* text-align: left; */
		margin: 0 auto;
	}

	h1 {
		margin: 0;
	}

	p {
		flex: 1;
		margin: 0 auto;
	}

	.flowers {
		font-size: x-large;
	}
	span {
		font-size: x-small;
	}

	.left {
		text-align: left;
	}
</style>
