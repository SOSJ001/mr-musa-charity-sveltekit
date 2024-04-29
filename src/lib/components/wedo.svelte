<script lang="ts">
	import Thingswedo from './thingswedo.svelte';
	import * as Icon from 'svelte-google-materialdesign-icons';
</script>

<div
	class="flex w-full gap-3 md:gap-0 flex-col items-center justify-between bg-[conic-gradient(at_top_left,_var(--tw-gradient-stops))] from-amber-600 via-transparent to-transparent p-5 px-10 md:flex-row"
>
	<div class="text-center md:w-1/2 text-xl md:text-[30px] font-bold">
		We Do It For People In Need
	</div>
	<div class="grid grid-cols-2 md:flex md:flex-row justify-center gap-5  md:w-1/2">
		<Thingswedo>
			<span slot="icon"><Icon.Medical_services variation="filled" class="" /></span>
			<span slot="description">Medicine Help</span>
		</Thingswedo>
		<Thingswedo>
			<span slot="icon"><Icon.Build class="" /></span>
			<span slot="description">Build Create</span>
		</Thingswedo>
		<Thingswedo>
			<span slot="icon"><Icon.Fastfood class="" /></span>
			<span slot="description">Food Help</span>
		</Thingswedo>
		<Thingswedo>
			<span slot="icon"><Icon.Sports class="" /></span>
			<span slot="description">Sport Enguagement</span>
		</Thingswedo>
	</div>
</div>
