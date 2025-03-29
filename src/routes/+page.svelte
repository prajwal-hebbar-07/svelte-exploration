<script lang="ts">
	let userName = $state('Existing User');
	$inspect(userName);

	// $effect(() => {
	//     console.log("Effect Hook")
	//     if(userName) {
	//         console.log(`Effect hook is performing an action on ${userName}`)
	//     }
	// })
</script>

<h1>Your Username:</h1>
<input type="text" bind:value={userName} />

<p>{userName}</p>
