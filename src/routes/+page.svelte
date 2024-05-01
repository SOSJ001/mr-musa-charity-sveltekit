<script>
	import Topnav from '$lib/components/topnav.svelte';
	import Heroimage from '$lib/components/heroimage.svelte';
	import Showcase from '$lib/components/showcase.svelte';
	import Wedo from '$lib/components/wedo.svelte';
	import Ourmission from '$lib/components/ourmission.svelte';
	import successstory from '$lib/images/against-light-7572922_1280.jpg';
	import news from '$lib/images/africa-news.jpg';
	import Gallery from '$lib/components/gallery.svelte';
	import Footer from '$lib/components/footer.svelte';


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

	<!-- News  -->
	<Showcase image={news} btn={false}>
		<div slot="title">News And Resources</div>
		<div slot="description">
			A group of resilient children gather, their faces telling stories
			of survival and hope. Despite the challenging circumstances they face daily, their spirits
			remain unbroken. Through local initiatives, these young souls are not only finding solace in
			sports and community activities but are also receiving essential support such as food,
			clothing, and medical care. These interventions aim to provide these children with the tools
			they need to build a promising future, proving that even in the toughest conditions, hope can
			thrive.
		</div>
	</Showcase>
	<!-- Our News ends -->

	<!-- Gallery -->
	<Gallery/>
	<!-- Gallery -->

	<!-- footer -->
<Footer/>
	<!-- footer -->
</div>
