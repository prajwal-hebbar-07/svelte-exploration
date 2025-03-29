<script lang="ts">
	let userName = $state('');
	let isEditMode = $state(false);
</script>

{#snippet userInput()}
	<h1>Your UserName:</h1>
	{#if isEditMode}
		<input type="text" bind:value={userName} />
	{:else}
		<p>{userName}</p>
	{/if}
{/snippet}

{@render userInput()}

<button onclick={() => (isEditMode = !isEditMode)}>{isEditMode ? 'Save Changes' : 'Edit'}</button>
