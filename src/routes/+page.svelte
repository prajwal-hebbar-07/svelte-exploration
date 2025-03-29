<script lang="ts">
    let userName = $state("")
</script>

<h1>Your Username:</h1>
<input type="text" bind:value={userName} />

<p>{userName}</p>