<script lang="ts">
	import sampler1 from '$lib/images/sampler-1.jpeg';
	import sampler2 from '$lib/images/sampler-2.jpeg';
	import sampler3 from '$lib/images/sampler-3.jpeg';
	import sampler4 from '$lib/images/sampler-4.jpeg';
	import Frame from '../atoms/Frame.svelte';
</script>

<Frame>
	<div>
		<p>
			NICOLETTE DOLAN 04.29.23 Thank you doe picking up my zine and being interested in my work!
			Endless thank yous to the Internet Archive and all of my friends who wanted to see mt put this
			into the world!
			<span>
				u can find my work and more at <a href="https://nicolettedolan.com">nicolettedolan.com</a>
			</span>
		</p>
		<section>
			<img alt="sampler 1" src={sampler1} />
			<img alt="sampler 2" src={sampler2} />
			<img alt="sampler 3" src={sampler3} />
			<img alt="sampler 4" src={sampler4} />
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
		display: grid;
		grid-template-columns: 1fr 1fr;
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
</style>
