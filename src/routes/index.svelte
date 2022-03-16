<script lang="ts">
	import Toggle from "$lib/Toggle.svelte";

	let isToggled = false;
</script>

<h1>Welcome to some Svelte-Components!</h1>

<section>
	<h2>Toggle</h2>
	<Toggle bind:isToggled label="This is the label" />
	<Toggle
		label="This is the label, styled"
		style="--toggleBackgroundColor: indianred; --toggleButtonColor: gray; --toggleCheckedBackgroundColor: teal;"
	/>

	{#if isToggled}
		<p>The first toggle is toggled!</p>
	{/if}
</section>
