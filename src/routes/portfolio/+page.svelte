<script lang="ts">
	import { Gallery } from "flowbite-svelte";

	const colImages1 = [
		{
			alt: "Siklab Sportsfest Day 1",
			src: "portfolio/DAY1.jpg",
		},
		{
			alt: "Siklab Sportsfest Day 2",
			src: "portfolio/DAY2.jpg",
		},
		{
			alt: "Siklab Sportsfest Day 3",
			src: "portfolio/DAY3.jpg",
		},
		{
			alt: "Siklab Sportsfest Day 4",
			src: "portfolio/DAY4.jpg",
		},
        {
			alt: "Sibul Kapihan 2",
			src: "portfolio/Sibul Kapihan 2.jpg",
		},
        {
			alt: "a wrap at connxt",
			src: "portfolio/74.jpg",
		},
        {
			alt: "fb vid",
			src: "portfolio/Le-galleria.jpg",
		},
	];

	const colImages2 = [
		{
			alt: "Paglalayag",
			src: "portfolio/paglalayag.jpg",
		},
		{
			alt: "Voltcon",
			src: "portfolio/voltcon.jpg",
		},
        {
			alt: "Connxt Bataan",
			src: "portfolio/GAKUEN-SAI.jpg",
		},
		{
			alt: "Sticker Gacha",
			src: "portfolio/stickergacha.jpg",
		},
		{
			alt: "World Teachers Day",
			src: "portfolio/happy world teachers day.jpg",
		},
        {
			alt: "Tryout",
			src: "portfolio/EMF album.jpg",
		},
        {
			alt: "Siklab Soar High",
			src: "portfolio/SIKLAB SCHED 1.jpg",
		},
        {
			alt: "Mr and Ms CCS",
			src: "portfolio/CONGRATS CCS.jpg",
		},
	];

	const colImages3 = [
		{
			alt: "Thank you CCS",
			src: "portfolio/SALAMAT CCS.jpg",
		},
		{
			alt: "photo at con",
			src: "portfolio/33.jpg",
		},
		{
			alt: "Banner",
			src: "portfolio/EMF Banner.jpg",
		},
        {
			alt: "1000 followers on Facebook",
			src: "portfolio/1000.jpg",
		},
        {
			alt: "prismatic burst",
			src: "portfolio/prismatic burst.jpg",
		},
	];

</script>

<div class="bg-black py-10">
	<div class="px-4 md:px-8">
		<h1 class="text-4xl text-orange-400 text-center">Portfolio</h1>
		<p class="text-center text-white mb-6">Here are some of my works, professional, freelance, and passion projects.</p>
	</div>
	<div class="w-full max-w-4xl mx-auto">
		<div class="grid gap-4 grid-cols-1 md:grid-cols-2 lg:grid-cols-4">
			<div class="flex flex-col gap-4">
				{#each colImages1 as colImage}
				<div class="w-full h-fit overflow-hidden rounded-lg">
					<img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
				</div>
				{/each}
			</div>
			<div class="flex flex-col gap-4">
				{#each colImages2 as colImage}
				<div class="w-full h-fit overflow-hidden rounded-lg">
					<img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
				</div>
				{/each}
			</div>
			<div class="md:col-span-2 flex flex-col gap-4">
				{#each colImages3 as colImage}
				<div class="w-full h-fit overflow-hidden rounded-lg">
					<img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
				</div>
				{/each}
			</div>
		</div>
	</div>
</div>
