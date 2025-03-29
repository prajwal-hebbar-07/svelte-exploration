<script lang="ts">
	import type { Snippet } from 'svelte';

	interface UserInputInterface {
		userName: string;
		children: Snippet;
	}
	let { userName, children, ...props }: UserInputInterface = $props();
</script>

<input type="text" bind:value={userName} />
<p>{userName}</p>
{@render children()}
