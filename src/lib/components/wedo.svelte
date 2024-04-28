<script lang="ts">
	import Thingswedo from './thingswedo.svelte';
    import * as Icon from 'svelte-google-materialdesign-icons';
    
    
</script>

<div class="mt-5 flex w-full items-center justify-between px-10 flex-col md:flex-row">
	<div class=" md:w-1/2 text-center gap-y-3 md:gap-y-0 text-[25px] md:text-[40px]">We Do It For People In Need</div>
	<div class="md:w-1/2 flex flex-row gap-5 justify-center">
		<Thingswedo>
            <span slot="icon"><Icon.Medical_services variation="filled" class="text-amber-600"/></span>
            <span slot="description">Medicine <br> help</span>
        </Thingswedo>
        <Thingswedo>
            <span slot="icon"><Icon.Build class="text-amber-600"/></span>
            <span slot="description">Build <br>Create</span>
        </Thingswedo>
        <Thingswedo>
            <span slot="icon"><Icon.Fastfood class="text-amber-600"/></span>
            <span slot="description">Food <br>Help</span>
        </Thingswedo>
        <Thingswedo>
            <span slot="icon"><Icon.Sports class="text-amber-600"/></span>
            <span slot="description">Sport <br>Enguagement</span>
        </Thingswedo>
	</div>
</div>
