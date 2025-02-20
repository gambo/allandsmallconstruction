<script lang="ts">
	import type { Snippet } from 'svelte';
	import Mail from 'lucide-svelte/icons/mail';

	type Props = {
		children: Snippet;
	};
	let { children }: Props = $props();
</script>

<div class="bg absolute inset-0 bg-slate-100">
	<div class="mx-auto w-1/2 pt-16 text-center">
		<div class="flex flex-col items-center gap-2 text-sm text-slate-800">
			<img src="/logo.svg" alt="All and Small Construction Logo" class="w-64" />
			<p class="pt-8 text-3xl text-pretty font-bold">Website under construction</p>
			<a href="mailto:clayton@allandsmallconstruction.com" class="flex gap-2 bg-gradient-to-b from-sky-700 to-sky-800 text-white text-xs px-5 py-3 items-center rounded-md shadow-lg mt-8">
				<Mail class="size-5" />
				<span>Send an Email for any queries.</span>
			</a>
		</div>
	</div>
</div>

<style lang="postcss">
	.bg {
		@apply bg-[url(/bg.jpg)];
	}
</style>
