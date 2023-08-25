<script lang="ts">
	import Frame from '../atoms/Frame.svelte';
	import wiki1 from '$lib/images/wiki-1.png';
	import wiki2 from '$lib/images/wiki-2.png';
</script>

<Frame>
	<div>
		<p>
			Sampler is a <sup>mostly done</sup> font based off of embroidery samplers found on the Internet
			Archive. A sampler is a piece of embroidery or cross-stitching produced as a specimen of achievement,
			demonstration or a test of skill in needlework. It often includes the alphabet, figures, motifs,
			decorative borders and sometimes the name of the person who embroidered it and the date. The word
			sampler is derived from the Latin exemplum, which means example.
		</p>
		<section>
			<img alt="wikipedia 1" src={wiki1} />
			<img alt="wikipedia 2" src={wiki2} />
			<small>Screenshots from the wikipedia page on Embroidery samplers</small>
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
		display: flex;
		flex-direction: column;
		flex: 1;
	}
	p {
		flex: 1;
		text-align: left;
		margin: 0 auto;
	}

	img {
		max-width: 100%;
		height: auto;
	}

	small {
		text-align: left;
	}
</style>
