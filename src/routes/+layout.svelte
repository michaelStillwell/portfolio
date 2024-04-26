<script>
	import "../app.postcss";
	import { AppShell, AppBar } from "@skeletonlabs/skeleton";
	import { filter, GreenFall } from "@skeletonlabs/skeleton";
	import Icon from "@iconify/svelte";
</script>

<GreenFall/>

<AppShell
	class="min-h-screen bg-gradient-to-b from-surface-900 to-tertiary-600"
>
	<svelte:fragment slot="header">
		<AppBar>
			<svelte:fragment slot="lead">
				<strong></strong>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<a
					class="text-2xl"
					href="mailto:contact@mstillwell.dev"
					target="_blank"
					rel="noreferrer"
				>
					<Icon icon="mage:email" />
				</a>
				<a
					class="text-2xl"
					href="https://github.com/michaelStillwell"
					target="_blank"
					rel="noreferrer"
				>
					<Icon icon="mage:github" />
				</a>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment>
	<!-- Page Route Content -->
	<slot />
</AppShell>
