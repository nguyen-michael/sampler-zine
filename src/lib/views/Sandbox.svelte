<script lang="ts">
	import Frame from '../atoms/Frame.svelte';

	const variants = ['regular', 'bold', 'light'] as const;

	const value = 'She was a garden at night...';

	let variant: (typeof variants)[number] = 'regular';
</script>

<Frame>
	<!-- svelte-ignore a11y-autofocus-->
	<textarea class={variant} autofocus {value} />
	<select name="variants" id="variants" bind:value={variant}>
		{#each variants as variant}
			<option value={variant}>{variant.toUpperCase()}</option>
		{/each}
	</select>
</Frame>

<style>
	textarea {
		width: 100%;
		height: 100%;
		word-wrap: break-word;
		border: none;
		font-size: 5rem;
		line-height: 7rem;
		font-family: 'Sampler';
		color: rgba(255, 255, 255, 0.87);
		background-color: #242424;
	}

	textarea.regular {
		font-weight: 400;
	}
	textarea.bold {
		font-weight: 700;
	}
	textarea.light {
		font-weight: 100;
	}

	textarea:focus {
		outline: none;
	}

	select {
		position: absolute;
		bottom: 0;
		right: 50%;
		transform: translateX(50%);

		border: none;
		font-family: 'Sampler';
	}
</style>
