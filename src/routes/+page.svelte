<script lang="ts">
	let userName = $state('');
</script>

{#snippet userInput()}
	<h1>Your UserName:</h1>
	<input type="text" bind:value={userName} />

	<p>{userName}</p>
{/snippet}

{@render userInput()}
