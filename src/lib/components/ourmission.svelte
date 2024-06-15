<script lang="ts">
	import img from '$lib/images/africamd.jpg';
	import img2 from '$lib/images/africa-1994846_1280.jpg';
</script>

<div
	class="relative my-5 flex items-center justify-center px-3 text-center font-mono font-bold md:h-[500px] md:px-10 md:text-xl"
>
	<div>
		<div class=" w-full">
			<img src={img} alt="mission" class="hidden rounded-xl md:block md:h-[500px]" />
		</div>
		<div class=" w-full">
			<img src={img2} alt="mission" class="h-[380px] rounded-xl md:hidden" />
		</div>
	</div>

	<div
		class="absolute flex h-full w-full items-center justify-center bg-slate-900 bg-opacity-30 md:p-10"
	>
		<div
			class="flex w-[300px] flex-col items-center justify-center rounded-xl bg-slate-900 bg-opacity-30 p-2 md:w-1/2 md:p-10"
		>
			<p class="m-2 text-xl md:text-[40px]">OUR MISSION</p>
			<p>
				"Mankind United to Save African Children (MUSAC) is committed to
				upholding the quality of services for children through health, education, and compassionate
				care. Our dedication lies in providing comprehensive support to African children, ensuring
				their holistic development and well-being."
			</p>
		</div>
	</div>
</div>
