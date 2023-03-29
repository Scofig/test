<script>
	import Block from '../Block.svelte';
	let colors = [
		{ bgcolor: 'red', opacity: 1 },
		{ bgcolor: 'blue', opacity: 1 },
		{ bgcolor: 'yellow', opacity: 1 },
		{ bgcolor: 'black', opacity: 1 },
		{ bgcolor: 'green', opacity: 1 }
	];
</script>

{#each colors as { bgcolor, opacity }}
	<Block
		{bgcolor}
		{opacity}
		on:click={() => {
			if (opacity) {
				colors.forEach((color) => (color.opacity = 1));
				opacity = 0;
			}
		}}
	/>
{/each}
