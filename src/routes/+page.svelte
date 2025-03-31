<script lang="ts">
	let peopleWaiting = $state(['121']);
</script>

<h1>Waiting Queue!</h1>

{#snippet queue(personId: string)}
	<li>ID of the Person Waiting: {personId}</li>
{/snippet}

<ul>
	{#each peopleWaiting as person}
		{@render queue(person)}
	{/each}
</ul>

<button onclick={() => peopleWaiting.push(new Date().getTime().toString())}>I'm Waiting!!</button>
