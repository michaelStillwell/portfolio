<script>
	import Card from "$lib/components/card.svelte";
</script>

<div class="px-4 h-full mx-auto">
	<section id="header" class="relative h-screen flex flex-col justify-center">
		<span class="z-10 text-right">
			<p class="text-2xl font-semibold text-secondary-500">
				Michael Stillwell
			</p>
			<h1 class="h1 text-primary-500 font-bold">
				Fullstack
				<br />
				Software Engineer
			</h1>
		</span>
	</section>

	<section id="about" class="">
		<h2 class="h2 mb-4">Who am I?</h2>
		<div class="flex justify-center">
			<Card
				title="Hello there!"
				body=" I am a fullstack software engineer with a passion for
						building web applications."
				footer="Rust · Js · C# · Svelte · React"
				footerAccent
			/>
		</div>
	</section>

	<section id="projects">
		<h2 class="h2 mb-4">Projects</h2>
		<div class="flex flex-wrap gap-2 justify-center">
			<Card
				title="Mane Witch"
				titleLink="https://www.manewitch.com/"
				body=" A company website for an awesome in-home salon based in Texas. "
				footer="Svelte | SkeletonUI | Vercel"
			/>

			<Card
				title="Pomodoro Timer"
				titleLink="https://pomodoro.mstillwell.dev/"
				body="A web based, vanilla Javascript pomodoro timer. You can set work and rest 
						times, and the values are saved to your browser so you don't have to 
						re-enter them when you return!"
				footer="Javascript | Vercel"
				footerLink="https://github.com/mstillwell/pomodoro"
			/>

			<Card
				title="List Maker"
				titleLink="https://list-maker.mstillwell.dev/"
				body="Create as many lists as you like with this tool! It includes a hand rolled 
						authentication strategy along side it, so you can save your lists for later!"
				footer="Svelte | SkeletonUI | Turso | Vercel"
				footerLink="https://github.com/mstillwell/list-maker"
			/>

			<Card
				title="Crabmat"
				titleLink="https://crates.io/crates/crabmat"
				body="A web based, vanilla Javascript pomodoro timer. You can set work and rest 
						times, and the values are saved to your browser so you don't have to 
						re-enter them when you return! It's been downloaded over 300 times!"
				footer="Rust | Ratatui"
				footerLink="https://github.com/mstillwell/crabmat"
			/>
		</div>
	</section>

	<section id="contact">
		<h2 class="h2">Contact me</h2>
		<div class="flex flex-col">
			<p>Want to work with me? Shoot me an email and we can talk!</p>
			<p>
				<b>Email: </b>
				<a class="underline" href="mailto:contact@mstillwell.dev">
					contact@mstillwell.dev
				</a>
			</p>
		</div>
	</section>

	<footer class="mb-6">
		<div class="flex flex-col justify-center items-center h-full">
			<p class="text-center text-gray-500 text-sm">
				<i> Stillwell Technologies </i> &copy; 2024
			</p>
		</div>
	</footer>
</div>

<style lang="postcss">
	section {
		@apply mb-64;
	}
</style>
