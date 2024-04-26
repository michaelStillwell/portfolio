<script>
	import Icon from "@iconify/svelte";

	/** @type {string} */
	export let title;
	/** @type {string} */
	export let titleLink = "#";

	/** @type {string} */
	export let body = "";

	/** @type {string} */
	export let footer = "";
	/** @type {string} */
	export let footerLink = "#";
	/** @type {boolean} */
	export let footerAccent = false;
</script>

<div class="w-[500px] flex flex-col justify-between bg-surface-800 rounded-lg">
	<span>
		<h3 class="h3 font-bold mb-3 pl-4 pt-4">
			<a class="underline" href={titleLink} target="_blank">
				{title}
			</a>
		</h3>
		<p class="p-4 mb-6 card-body">
			{body}
		</p>
	</span>

	<span class:accented={footerAccent} class:not-accented={!footerAccent}>
		{#if footerLink.length > 1}
			<a href={footerLink} target="_blank">
				<Icon icon="mage:github" />
			</a>
		{/if}
		{footer}
	</span>
</div>

<style lang="postcss">
	.accented {
		@apply bg-primary-500;
		@apply font-bold;
		@apply rounded-xl;
		@apply text-center;
		@apply mt-2;
		@apply py-2;
		@apply m-4;
	}
	.not-accented {
		@apply flex;
		@apply gap-4;
		@apply card-footer;
		@apply justify-self-end;
		@apply text-sm;
	}
	.not-accented a {
		@apply text-base;
	}
</style>
