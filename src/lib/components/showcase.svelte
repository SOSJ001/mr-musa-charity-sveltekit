<script lang="ts">
	import together from '$lib/images/children-5833685_1280.jpg';
	import Button from '$lib/components/button.svelte';
	export let order: string = 'last';
</script>

<div class="flex flex-col w-full items-center justify-between gap-5 p-3 text-gray-300 md:flex-row md:px-10 my-5">
    <!-- text below  -->
	<div class="w-full md:w-1/2 space-y-3">
		<p class=" text-center hidden md:block font-bold text-amber-600 text-[20px] md:text-[40px]">
			Helping Each Other Can Make World Better
		</p>
        <p class="md:hidden text-center font-bold text-amber-600 text-[20px]">
			Helping Each Other Can Make World Better
		</p>
		<p class="text-lg">
			While we take a moment to appreciate how far we've come, we also look forward to the path
			ahead. There are still many lives waiting for a beacon of hope, and with your continued
			support, we can reach even further. Each contribution empowers us to expand our outreach and
			deepen our impact.
		</p>
		<div class=" hidden space-x-5 md:block">
			<Button btnstyle="rounded-lg bg-amber-600 p-2 font-bold text-slate-900 hover:bg-amber-500">
				Our Mission
			</Button>
			<Button
				btnstyle="rounded-lg border border-amber-600 p-2 font-bold hover:border-gray-300 hover:text-amber-500"
			>
				Our Vision
			</Button>
		</div>
	</div>

    <!-- image below -->
	<div class="w-full md:w-1/2 order-{order}"><img class="rounded-xl" src={together} alt="together" /></div>
</div>
