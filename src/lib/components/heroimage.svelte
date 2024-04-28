<script>
	import heroimagemd from '$lib/images/africa-2002835_1280.jpg';
	import heroimagesm from '$lib/images/heroimage.jpg';
	import Button from './button.svelte';
</script>

<div class="relative w-full md:h-[550px]">
	<img class="hidden h-[550px] w-full md:block" src={heroimagemd} alt="hero of boy" />
	<img class="w-full md:hidden" src={heroimagesm} alt="hero of boy" />

	<div
		class="left-0 top-0 absolute flex h-full w-full flex-col items-start justify-center gap-y-4 bg-gradient-to-r from-slate-900 via-transparent to-transparent p-3 md:p-10 font-mono text-amber-600 "
	>
		<div class="flex flex-col md:text-[50px]">
			<span class="">Helping Special</span>
			<span class="">Individuals</span>
		</div>
		<div class="w-[150px] md:w-[400px] font-mono space-y-4">
			<div class="text-xs md:text-lg text-gray-300">
				<span class="">
					Your support has the power to make a real difference in someone's life.
				</span>
			</div>
			<div>
				<Button
					btnstyle="rounded-lg text-xs md:text-lg bg-amber-600 p-2 font-bold text-slate-900 hover:bg-amber-500"
				>
					Donate a meal
				</Button>
			</div>
			<div class=" text-xs text-gray-300 space-y-3">
				<p class="text-xs md:text-lg border-l-2 border-amber-600 pl-3">1.2K Lives Changed and Counting...</p>
                <p class="hidden md:block"> Your support transforms lives. Each number here reflects
				a story of hope and resilience. Together, we can reach the next thousand. Join the
				movement—every contribution creates a ripple of lasting impact.</p>
			</div>
		</div>
	</div>
</div>
