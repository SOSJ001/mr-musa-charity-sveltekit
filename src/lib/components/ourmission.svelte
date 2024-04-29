<script lang="ts">
    import img from "$lib/images/africamd.jpg"
    import img2 from "$lib/images/africa-1994846_1280.jpg"

</script>

<div
	class="relative flex items-center justify-center my-5 px-3 text-center font-mono font-bold md:px-10 md:text-xl md:h-[500px]"
>
	<div>
        <div class=" w-full"><img src={img} alt="mission" class="md:h-[500px] hidden md:block rounded-xl" /></div>
	<div class=" w-full"><img src={img2} alt="mission" class="md:hidden rounded-xl" /></div>
    </div>

	<div class="absolute bg-slate-900 bg-opacity-30 md:p-10 h-full w-full flex items-center justify-center">
        <div class="w-[300px] md:w-1/2 flex flex-col items-center justify-center bg-slate-900 p-2 md:p-10 rounded-xl bg-opacity-30">
            <p class="text-xl">OUR MISSION</p>
		<p>
			"Is to nurture hope among African children by engaging them through sports, while also
			providing essential nourishment, clothing, and medical care to support their well-being and
			bright futures."
		</p>
        </div>
		
	</div>
</div>
