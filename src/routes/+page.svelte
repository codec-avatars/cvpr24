<script lang="ts">
	// External Libraries
	import FaTwitter from 'svelte-icons/fa/FaTwitter.svelte';
	import FaLinkedinIn from 'svelte-icons/fa/FaLinkedinIn.svelte';
	import FaYoutube from 'svelte-icons/fa/FaYoutube.svelte';
	import FaFilePdf from 'svelte-icons/fa/FaFilePdf.svelte';
	import FaGithub from 'svelte-icons/fa/FaGithub.svelte';
	import { base } from "$app/paths";
	
	// Flowbite
	import { Navbar, NavBrand, NavLi, NavUl, Button, NavHamburger } from 'flowbite-svelte'
  
	let datasetName = 'Aurora Multi-Sensor Dataset';

</script>  

<svelte:head>
	<title>Codec Avatars Workshop @ CVPR'24</title>
</svelte:head>


<!-- <header class="bg-white">
	<div class="max-w-screen-l flex flex-wrap items-center justify-between mx-auto">
		
		<nav>
			<ul class="flex space-x-6">
				<li><a href="#" class="text-gray-600 hover:text-gray-900">Home</a></li>
				<li>
					<a " class="text-white bg-blue-600 hover:bg-blue-700 px-4 py-2 rounded">
						
					</a>
				</li>
			</ul>
		</nav>
	</div>
</header> -->

<Navbar let:hidden let:toggle>
	<div class="text-xl font-semibold">Codec Avatars @ CVPR24</div>
	<!-- <NavBrand href="/">
		<img
		src="/images/flowbite-svelte-icon-logo.svg"
		class="mr-3 h-6 sm:h-9"
		alt="Flowbite Logo"
		/>
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
		Flowbite
		</span>
	</NavBrand> -->
	<!-- <div class="flex md:order-2">
		<Button size="sm" href="https://github.com/pit30m/pit30m">Download Dataset</Button>
		<NavHamburger on:click={toggle} />
	</div> -->
	<NavUl {hidden}>
		<NavLi href="{base}/" active={true}>Home</NavLi>
		<NavLi href="{base}/">Overview</NavLi>
		<NavLi href="{base}/">Schedule</NavLi>
		<NavLi href="{base}/">Speakers</NavLi>
		<NavLi href="{base}/">Organizers</NavLi>
	</NavUl>
</Navbar>


<body>
<!-- Background image 1 from https://unsplash.com/photos/F6Kj8ovnUvM -->
<!-- Background image 2 from https://unsplash.com/photos/yLcPSvJkGrM -->
<!-- <section class="bg-cover bg-center h-96 relative" style="background-image: url('hero_bg.jpg')"> -->

<section class="bg-white dark:bg-gray-900">
    <div class="py-8 px-4 mx-auto max-w-screen-xl text-center lg:py-16 lg:px-12">
        
        <h1 class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-gray-900 md:text-5xl lg:text-6xl dark:text-white">
			Workshop on Codec Avatars @ CVPR24
		</h1>
        <p class="mb-8 text-lg font-normal text-gray-500 lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
			Full-day workhsop on Tuesday, June 18, 2024, at the Seattle Convention Center.
		</p>
        
    </div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white">Overview</h2>
		<div class="pt-4"><p class="text-xl">
			Our workshop will be devoted to telepresence: the task of generating and driving realistic human representations. 
			Regarding generation, we plan to cover the learning of efficient 3d representations of faces, hands, and bodies, and the particular challenges of each modality. 
			For driving, we will focus on using headsets to drive faces and hands, as well as external cameras for full-body tracking. 
			The invited speakers will provide context on the state of the art both in industry and academia for efficient 3d representations and their applications to human modelling.
		</div>
	</div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white">Schedule</h2>
		<div class="pt-4"><p class="text-xl">
			Coming soon.
		</div>
	</div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white">Speakers</h2>
		<div class="pt-4"><p class="text-xl">
			Coming soon.
		</div>
	</div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white">Organizers</h2>
		<div class="pt-4"><p class="text-xl">
			Coming soon.
		</div>
	</div>
</section>

</body>


<footer class="bg-gray-200 py-8 mt-8">
	<div class="container mx-auto px-4">
		<div class="flex justify-between items-center">

			<div class="text-gray-600">
				<p>
					Email: <a href="mailto:julietamartinez@meta.com" class="hover:text-gray-900">julietamartinez@meta.com</a>
				</p>
			</div>
			<div class="text-center text-gray-600">
				<p>&copy; 2024. All rights reserved.</p>
			</div>
		</div>
	</div>
</footer>



<style>
	.icon {
		display: inline-block;
		font-size: inherit;
		height: 1em;
		overflow: visible;
		vertical-align: -0.125em;
	}
</style>
