<script>
	import { Gallery } from 'flowbite-svelte';
	import images001 from '$lib/images/africa-1994846_1280.jpg';
	import images002 from '$lib/images/children-7832777_1280.jpg';
	import images003 from '$lib/images/africa-news.jpg';
	import images004 from '$lib/images/heroimage.jpg';
	import images005 from '$lib/images/against-light-7572922_1280.jpg';
	import images006 from '$lib/images/children-5833685_1280.jpg';
	import images007 from '$lib/images/children-200066_1280.jpg';
	import images008 from '$lib/images/children-331234_1280.jpg';

	const images1 = [
		{ alt: 'erbology', src: images001 },
		{ alt: 'small bag', src: images003 }
	];
	const images2 = [
		{ alt: 'erbology', src: images004 },
		{ alt: 'shoes', src: images005 }
	];
	const images3 = [
		{ alt: 'small bag', src: images006 },
		{ alt: 'shoes', src: images002 }
	];
	const images4 = [
		{ alt: 'erbology', src: images008 },
		{ alt: 'small bag', src: images007 }
	];
</script>

<div class="space-y-3 p-3 text-center md:px-10">
	<div class="text-3xl font-bold text-amber-600">Gallery</div>
	<Gallery class="grid-cols-2 gap-4 md:grid-cols-4 ">
		<Gallery items={images1} />
		<Gallery items={images2} />
		<Gallery items={images3} />
		<Gallery items={images4} />
	</Gallery>
</div>
