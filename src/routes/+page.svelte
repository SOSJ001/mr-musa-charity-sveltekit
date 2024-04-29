<script>
	import Topnav from '$lib/components/topnav.svelte';
	import Heroimage from '$lib/components/heroimage.svelte';
	import Showcase from '$lib/components/showcase.svelte';
	import Wedo from '$lib/components/wedo.svelte';
	import Ourmission from '$lib/components/ourmission.svelte';
	import successstory from '$lib/images/against-light-7572922_1280.jpg';
</script>

<div class="h-screen w-screen overflow-x-hidden bg-slate-900 font-serif text-white">
	<!-- topnav below -->
	<Topnav />
	<!-- topnav ends -->

	<!-- heroimage below -->
	<Heroimage />
	<!-- heroimage ends -->

	<!-- showcase below -->
	<Showcase />
	<!-- showcase ends -->

	<!-- wedo below -->
	<Wedo />
	<!-- wedo ends -->

	<!-- Our Mission below -->
	<Ourmission />
	<!-- Our Mission ends -->

	<!-- Our Success Story below -->
	<Showcase order="first" image={successstory} btn={false}>
		<div slot="title">Our Success Story</div>
		<div slot="description">
            "Since our inception, we have seen countless lives transformed through our collective efforts.
			In the heart of Africa, we've ignited a spark of change one child, one game, one meal at a
			time. Our sports programs have cultivated discipline and joy, nourishing both the body and
			spirit of the young athletes. Beyond the field, our initiative has clothed, fed, and healed,
			extending a lifeline to those in dire need. These victories aren't just ours, they belong to
			every supporter who believed in the cause. Together, we have sown seeds of hope that will
			bloom for generations to come."
			
		</div>
	</Showcase>
	<!-- Our Success Story ends -->
</div>
