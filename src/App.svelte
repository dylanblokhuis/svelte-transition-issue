<script>
	import { fade } from 'svelte/transition';

	let visible = true;
</script>

<svelte:options tag="my-component" />

<label>
	<input type="checkbox" bind:checked={visible}>
	visible
</label>

{#if visible}
	<p transition:fade>
		Fades in and out
	</p>
{/if}

