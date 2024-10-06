<script lang="ts">
	import { Gallery } from "flowbite-svelte";
  
	const colImages1 = [
	  { alt: "Siklab Sportsfest Day 1", src: "portfolio/DAY1.jpg" },
	  { alt: "Siklab Sportsfest Day 2", src: "portfolio/DAY2.jpg" },
	  { alt: "Siklab Sportsfest Day 3", src: "portfolio/DAY3.jpg" },
	  { alt: "Siklab Sportsfest Day 4", src: "portfolio/DAY4.jpg" },
	  { alt: "Sibul Kapihan 2", src: "portfolio/Sibul Kapihan 2.jpg" },
	  { alt: "a wrap at connxt", src: "portfolio/74.jpg" },
	  { alt: "fb vid", src: "portfolio/Le-galleria.jpg" },
	  { alt: "Adobe XD Mobile Connection", src: "portfolio/Adobe XD (2).png" },
	];
  
	const colImages2 = [
	  { alt: "Paglalayag", src: "portfolio/paglalayag.jpg" },
	  { alt: "Voltcon", src: "portfolio/voltcon.jpg" },
	  { alt: "Connxt Bataan", src: "portfolio/GAKUEN-SAI.jpg" },
	  { alt: "Sticker Gacha", src: "portfolio/stickergacha.jpg" },
	  { alt: "Blogpost Info Management", src: "portfolio/blogpost info management.png" },
	  { alt: "Website Intro to HCI", src: "portfolio/website intro to hci.png" },
	  { alt: "Siklab Soar High", src: "portfolio/SIKLAB SCHED 1.jpg" },
	  { alt: "Mr and Ms CCS", src: "portfolio/CONGRATS CCS.jpg" },
	  { alt: "GC Library Management System", src: "portfolio/fordan lms.PNG" },
	  { alt: "Adobe XD PC Connection", src: "portfolio/Adobe XD (1).png" },
	];
  
	const colImages3 = [
	  { alt: "Thank you CCS", src: "portfolio/SALAMAT CCS.jpg" },
	  { alt: "photo at con", src: "portfolio/33.jpg" },
	  { alt: "OOP Delivery Management", src: "portfolio/delivery management.png" },
	  { alt: "Animation", src: "portfolio/Scaffold3-Fordan.jpg" },
	  { alt: "sjc oc characters", src: "portfolio/sjc oc characters.png" },
	  { alt: "SJC School Brochure", src: "portfolio/School Brochure - Module 4.png" },
	  { alt: "Siklab", src: "portfolio/Videos (1).gif" },
	  { alt: "CCS Week", src: "portfolio/Videos (2).gif" },
	  { alt: "Paglalayag", src: "portfolio/Videos (3).gif" },
	];
  </script>
  
  <style>
	/* Animation Keyframes */
	@keyframes fadeIn {
	  0% {
		opacity: 0;
		transform: scale(0.95);
	  }
	  100% {
		opacity: 1;
		transform: scale(1);
	  }
	}
  
	/* Apply Animation */
	.fade-in {
	  opacity: 0;
	  animation: fadeIn 0.7s ease forwards;
	}
  
	/* Delay each element slightly for a cascading effect */
	.fade-in:nth-child(1) {
	  animation-delay: 0.2s;
	}
	.fade-in:nth-child(2) {
	  animation-delay: 0.4s;
	}
	.fade-in:nth-child(3) {
	  animation-delay: 0.6s;
	}
	.fade-in:nth-child(4) {
	  animation-delay: 0.8s;
	}
	.fade-in:nth-child(5) {
	  animation-delay: 1s;
	}
  
	img:hover {
  		transform: scale(1.1);
  		transition: transform 0.3s ease;
	}

  </style>
  
  <div class="bg-black py-40">
	<div class="px-4 md:px-8">
	  <h1 class="text-4xl text-orange-400 font-bold text-center">Projects</h1>
	  <p class="text-center text-white mb-6">
		Most of the projects I'm showing are mostly previous works in school from Junior High, Senior High, to College. 
		Things like school events, conventions, infographs, assignments and many many more are here. Here's the following:
	  </p>
	</div>
  
	<div class="w-full max-w-4xl mx-auto">
	  <div class="grid gap-4 grid-cols-1 md:grid-cols-2 lg:grid-cols-2">
		<!-- Column 1 -->
		<div class="flex flex-col gap-4">
		  {#each colImages1 as colImage}
		  <div class="w-full h-fit overflow-hidden rounded-lg fade-in">
			<img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
		  </div>
		  {/each}
		</div>
  
		<!-- Column 2 -->
		<div class="flex flex-col gap-4">
		  {#each colImages2 as colImage}
		  <div class="w-full h-fit overflow-hidden rounded-lg fade-in">
			<img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
		  </div>
		  {/each}
		</div>
  
		<!-- Column 3  -->
		<div class="md:col-span-2 flex flex-col gap-4">
		  {#each colImages3 as colImage}
		  <div class="w-full h-fit overflow-hidden rounded-lg fade-in">
			<img src={colImage.src} alt={colImage.alt} class="w-full hover:scale-110 transition-transform duration-300" loading="lazy">
		  </div>
		  {/each}
		</div>
	  </div>
	</div>
  </div>
  