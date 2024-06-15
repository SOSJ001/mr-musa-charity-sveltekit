<script>
	import { CloseButton, Drawer, Navbar, NavBrand } from 'flowbite-svelte';
	import { sineIn } from 'svelte/easing';
	import Button from './button.svelte';
	let hidden2 = true;
	let spanClass = 'flex-1 ms-3 whitespace-nowrap';
	let transitionParams = {
		x: -320,
		duration: 200,
		easing: sineIn
	};
</script>

<Navbar class=" border-b-2 border-amber-600 bg-slate-900 text-white">
	<NavBrand href="/">
		<img src="" class="me-3 h-6 sm:h-9" alt="MUSAC Logo" />
		<span class="self-center whitespace-nowrap text-xl font-semibold">logo</span>
	</NavBrand>
	<div class="flex md:order-2">
		<div class=" hidden space-x-5 md:block">
			<Button btnstyle="rounded-lg bg-amber-600 p-2 font-bold text-slate-900 hover:bg-amber-500">
				Donate
			</Button>
			<Button btnstyle="rounded-lg border border-amber-600 p-2 font-bold hover:border-gray-300 hover:text-amber-500">
				Contact
			</Button>
		</div>
		<button class="md:hidden" on:click={() => (hidden2 = false)}>
			<svg
			class="text-white h-6"
				xmlns="http://www.w3.org/2000/svg"
				x="0px"
				y="0px"
				viewBox="0 0 50 50"
				fill="currentcolor"
			>
				<path
					d="M 5 8 A 2.0002 2.0002 0 1 0 5 12 L 45 12 A 2.0002 2.0002 0 1 0 45 8 L 5 8 z M 5 23 A 2.0002 2.0002 0 1 0 5 27 L 45 27 A 2.0002 2.0002 0 1 0 45 23 L 5 23 z M 5 38 A 2.0002 2.0002 0 1 0 5 42 L 45 42 A 2.0002 2.0002 0 1 0 45 38 L 5 38 z"
				></path>
			</svg>
		</button>
	</div>
	<div class="hidden space-x-5 md:block">
		<a class="hover:text-amber-500" href="/">Home</a>
		<a class="hover:text-amber-500" href="/">About</a>
		<a class="hover:text-amber-500" href="/">News</a>
		<a class="hover:text-amber-500" href="/">Gallery</a>

	</div>
	<Drawer
		class="w-64 border-r border-amber-500 bg-slate-900 text-gray-300"
		transitionType="fly"
		{transitionParams}
		bind:hidden={hidden2}
		id="sidebar2"
	>
		<div class="flex items-center border-b border-amber-500">
			<h5
				id="drawer-navigation-label-3"
				class="text-base font-semibold uppercase text-gray-500 dark:text-gray-400"
			>
				Menu
			</h5>
			<CloseButton on:click={() => (hidden2 = true)} class="mb-4 dark:text-white" />
		</div>
		<div class=" flex flex-col items-center justify-between space-y-5 pt-5 md:hidden">
			<a class="hover:text-amber-500" href="/">Home</a>
			<a class="hover:text-amber-500" href="/">About</a>
			<a class="hover:text-amber-500" href="/">News</a>
			<a class="hover:text-amber-500" href="/">Gallery</a>

		</div>
	</Drawer>
</Navbar>
