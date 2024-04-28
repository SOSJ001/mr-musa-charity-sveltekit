<script>
	import heroimagemd from '$lib/images/africa-2002835_1280.jpg';
	import heroimagesm from '$lib/images/heroimage.jpg';
	import Button from './button.svelte';
</script>

<div class="relative w-full md:h-[550px]">
	<img class="hidden h-[550px] w-full md:block" src={heroimagemd} alt="hero of boy" />
	<img class="w-full md:hidden" src={heroimagesm} alt="hero of boy" />

	<!-- Text on image below and gradient below -->
	<div
		class="absolute left-0 top-0 flex h-full w-full flex-col items-start justify-center gap-y-4 bg-gradient-to-r from-slate-900 via-transparent to-transparent  font-mono text-amber-600 p-3 md:p-10"
	>
		<div class="flex flex-col md:text-[50px] font-bold">
			<span class="">Helping Special</span>
			<span class="">Individuals</span>
		</div>
		<div class="w-[150px] space-y-4 font-mono md:w-[400px]">
			<div class="text-xs text-gray-300 md:text-lg">
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
			<div class=" space-y-3 text-xs text-gray-300">
				<p class="border-l-2 border-amber-600 pl-3 text-xs md:text-lg">
					1.2K Lives Changed and Counting...
				</p>
				<p class="hidden md:block">
					A journey of small steps and giant leaps, of challenges overcome and successes celebrated.
					We want to thank you for being an integral part of this journey. Your trust and
					participation have been the driving force behind every life that's been changed for the
					better.
				</p>
			</div>
		</div>
	</div>
</div>
