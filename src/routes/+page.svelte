<script>
	import Topnav from '$lib/components/topnav.svelte';
	import Heroimage from '$lib/components/heroimage.svelte';
	import Showcase from '$lib/components/showcase.svelte';
	import Showcaseleft from '$lib/components/showcaseleft.svelte';
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

	<!-- Commitment -->
	<Showcaseleft image={successstory} btn={false}>
		<div slot="title">Commitment</div>
		<div slot="description">
			"MUSAC, we are steadfastly committed to improving the lives of African children by addressing
			their health needs, nurturing their educational journey, and offering compassionate care. Our
			unwavering dedication drives us to uphold the highest standards of service delivery, fostering
			a nurturing environment where every child can thrive."
		</div>
	</Showcaseleft>
	<!-- Commitment -->

	<!-- Vision  -->
	<Showcase image={news} btn={false}>
		<div slot="title">Vision</div>
		<div slot="description">
			Our vision at MUSAC is to grow, nurture, and contribute meaningfully to society by empowering
			African children with the resources, support, and opportunities they need to succeed. Through
			our efforts, we envision a future where every child in Africa has access to quality
			healthcare, education, and a nurturing environment, enabling them to reach their full
			potential.
		</div>
	</Showcase>
	<!-- Vision ends -->

	<!-- Specialization -->
	<Showcaseleft image={successstory} btn={false}>
		<div slot="title">Specialization</div>
		<div slot="description">
			We specialize in addressing crucial aspects of child health, including ear, eye, and childhood
			diseases. By focusing on these areas, we aim to alleviate suffering, improve quality of life,
			and ensure a brighter future for the children we serve.
		</div>
	</Showcaseleft>
	<!-- Specialization ends -->

	<!-- Gallery -->
	<Gallery />
	<!-- Gallery -->

	<!-- footer -->
	<Footer />
	<!-- footer -->
</div>
