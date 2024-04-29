<script lang="ts">
	import Thingswedo from './thingswedo.svelte';
    import * as Icon from 'svelte-google-materialdesign-icons';
    
    
</script>

<div class="bg-[conic-gradient(at_top_left,_var(--tw-gradient-stops))] from-amber-600 via-transparent to-transparent flex w-full items-center justify-between px-10 flex-col md:flex-row p-5">
	<div class=" md:w-1/2 text-center gap-y-3 md:gap-y-0 text-[25px] md:text-[40px]">We Do It For People In Need</div>
	<div class="md:w-1/2 flex flex-row gap-5 justify-center">
		<Thingswedo>
            <span slot="icon"><Icon.Medical_services variation="filled" class=""/></span>
            <span slot="description">Medicine <br> Help</span>
        </Thingswedo>
        <Thingswedo>
            <span slot="icon"><Icon.Build class=""/></span>
            <span slot="description">Build <br>Create</span>
        </Thingswedo>
        <Thingswedo>
            <span slot="icon"><Icon.Fastfood class=""/></span>
            <span slot="description">Food <br>Help</span>
        </Thingswedo>
        <Thingswedo>
            <span slot="icon"><Icon.Sports class=""/></span>
            <span slot="description">Sport <br>Enguagement</span>
        </Thingswedo>
	</div>
</div>
