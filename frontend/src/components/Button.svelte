<script lang="ts">
	import type { Snippet } from 'svelte';

	interface ButtonProps {
		children: Snippet;
	}
	let { children }: ButtonProps = $props();
</script>

<button
	class="rounded-md bg-transparent hover:bg-slate-200 text-zinc-200 hover:text-black font-bold text-xl align-center w-1/6 hover: transition-colors"
>
	{@render children()}
</button>
