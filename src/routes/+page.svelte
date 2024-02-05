<script lang="ts">
	// External Libraries
	import FaTwitter from 'svelte-icons/fa/FaTwitter.svelte';
	import FaLinkedinIn from 'svelte-icons/fa/FaLinkedinIn.svelte';
	import FaYoutube from 'svelte-icons/fa/FaYoutube.svelte';
	import FaFilePdf from 'svelte-icons/fa/FaFilePdf.svelte';
	import FaGithub from 'svelte-icons/fa/FaGithub.svelte';
	import YouTube from 'svelte-youtube-embed';
	import { base } from "$app/paths";
	
	// Flowbite
	import { Navbar, NavBrand, NavLi, NavUl, Button, NavHamburger } from 'flowbite-svelte'
  
	let datasetName = 'Aurora Multi-Sensor Dataset';

</script>  

<svelte:head>
	<title>Aurora Multi-Sensor Dataset</title>
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
	<div class="text-xl font-semibold">{datasetName}</div>
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
	<div class="flex md:order-2">
		<Button size="sm" href="https://github.com/pit30m/pit30m">Download Dataset</Button>
		<NavHamburger on:click={toggle} />
	</div>
	<NavUl {hidden}>
		<NavLi href="https://github.com/pit30m/pit30m" active={true}>DevKit</NavLi>
		<NavLi href="https://youtu.be/hJ6A_1YSITo">Video</NavLi>
		<NavLi href="https://arxiv.org/abs/2012.12437">Paper</NavLi>
	</NavUl>
</Navbar>



<body>
<!-- Background image 1 from https://unsplash.com/photos/F6Kj8ovnUvM -->
<!-- Background image 2 from https://unsplash.com/photos/yLcPSvJkGrM -->
<!-- <section class="bg-cover bg-center h-96 relative" style="background-image: url('hero_bg.jpg')"> -->

<section class="bg-white dark:bg-gray-900">
    <div class="py-8 px-4 mx-auto max-w-screen-xl text-center lg:py-16 lg:px-12">
        
        <h1 class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-gray-900 md:text-5xl lg:text-6xl dark:text-white">
			{datasetName}: The Largest Self-Driving Dataset Released to Date
		</h1>
        <p class="mb-8 text-lg font-normal text-gray-500 lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
			<a class="text-blue-600 hover:underline" href="https://una-dinosauria.github.io/">Julieta Martinez</a><sup>1</sup>
			<a class="text-blue-600 hover:underline" href="https://www.cs.toronto.edu/~doubovs/">Sasha Doubov</a><sup>1,2</sup>, 
			Jack Fan<sup>1</sup>, 
			<a class="text-blue-600 hover:underline" href="https://siegedog.com/">Ioan Andrei Bârsan</a><sup>1,3</sup>, 
			<a class="text-blue-600 hover:underline" href="https://shenlong.web.illinois.edu/">Shenlong Wang</a><sup>1,3</sup>, 
			Gellért Máttyus<sup>1</sup>, 
			<a class="text-blue-600 hover:underline" href="http://www.cs.toronto.edu/~urtasun/">Raquel Urtasun</a><sup>1,3</sup>
		</p>
		<p class="mb-8 text-lg font-normal text-gray-500 lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
			<sup>1</sup>Uber Advanced Technologies Group
			<sup>2</sup>University of Waterloo
			<sup>3</sup>University of Toronto
		</p>
        <div class="flex flex-col mb-8 lg:mb-16 space-y-4 sm:flex-row sm:justify-center sm:space-y-0 sm:space-x-4">
            <a href="https://arxiv.org/abs/2012.12437" class="inline-flex justify-center items-center py-3 px-5 text-base font-medium text-center text-white rounded-lg bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900">
                Paper
                <svg class="ml-2 -mr-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
					<FaFilePdf />
				</svg>
            </a>
			<a href="https://github.com/pit30m/pit30m" class="inline-flex justify-center items-center py-3 px-5 text-base font-medium text-center text-white rounded-lg bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900">
                DevKit
                <svg class="ml-2 -mr-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
					<FaGithub />
				</svg>
            </a>
            <a href="https://youtu.be/hJ6A_1YSITo" class="inline-flex justify-center items-center py-3 px-5 text-base font-medium text-center text-gray-900 rounded-lg border border-gray-300 hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800">
                <svg class="mr-2 -ml-1 w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
					<FaYoutube />	
				</svg>
                Watch video
            </a>  
        </div>
        
    </div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white">Video</h2>
		<!-- <p class="text-xl"></p> -->
		<!-- <br /> -->
		<div class="pt-4">
			<YouTube id="hJ6A_1YSITo" />
		</div>
	</div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white">Abstract</h2>
		<div class="pt-4"><p class="text-xl">
			We are interested in understanding whether retrieval-based localization approaches are good enough in the context of self-driving vehicles. Towards this goal, we introduce Pit30M, a new image and LiDAR dataset with over 30 million frames, which is 10 to 100 times larger than those used in previous work. Pit30M is captured under diverse conditions (i.e., season, weather, time of the day, traffic), and provides accurate localization ground truth. We also automatically annotate our dataset with historical weather and astronomical data, as well as with image and LiDAR semantic segmentation as a proxy measure for occlusion. We benchmark multiple existing methods for image and LiDAR retrieval and, in the process, introduce a simple, yet effective convolutional network-based LiDAR retrieval method that is competitive with the state of the art. Our work provides, for the first time, a benchmark for sub-metre retrieval-based localization at city scale.</p>
			<!-- The dataset, additional experimental results, as well as more information about the sensors, calibration, and metadata, are available on the project website: this https URL</p> -->
		</div>
	</div>
</section>

<section class="container mx-auto px-4 py-12">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white">Paper (IROS 2020 Best Application Paper Finalist)</h2>
		<div class="pt-4">
			<a href="https://arxiv.org/abs/2012.12437">
				<img src="combined.jpeg" alt="paper"/>
			</a>
		</div>
	</div>
</section>


<section class="container mx-auto px-4 py-12">
	<div class="grid overflow-x-auto">
		<h2 class="text-4xl font-extrabold dark:text-white">BibTeX</h2>
		<div class="text-lg pt-4">If you find our dataset useful, consider citing our work:
			<div class="bg-gray-100">
				<pre><code>{`
  @inproceedings{martinez2020pit30m,
	title={Pit30m: A benchmark for global localization in the age of self-driving cars},
	author={Martinez, Julieta and Doubov, Sasha and Fan, Jack and B{\^a}rsan, Ioan Andrei and Wang, Shenlong and 
	  M{\'a}ttyus, Gell{\'e}rt and Urtasun, Raquel},
	booktitle={{IROS}},
	pages={4477--4484},
	year={2020},
	organization={IEEE}
  }`}
				</code></pre>
			</div>
		</div>
	</div>
</section>

</body>

<footer class="bg-gray-200 py-8">
	<div class="container mx-auto px-4">
		<div class="flex justify-between items-center">
			<div class="text-gray-600">
				<a href="https://github.com/user/repo" class="mr-4 hover:text-gray-900">GitHub</a>
				<a href="https://youtu.be/video-url" class="mr-4 hover:text-gray-900">Video</a>
				<a href="https://arxiv.org/abs/paper-url" class="hover:text-gray-900">Paper</a>
			</div>
			<div class="text-gray-600">
				<p>
					Email:
					<a href="mailto:info@pit30m.com" class="hover:text-gray-900">info@pit30m.com</a>
				</p>
				<div class="flex space-x-4 mt-4">
					<a href="https://twitter.com/andreib" class="text-gray-600 hover:text-gray-900">
						<div class="icon text-gray-600">
							<FaTwitter />
						</div>
					</a>
					<a href="https://linkedin.com/company/pit30m" class="text-gray-600 hover:text-gray-900">
						<div class="icon text-gray-600">
							<FaLinkedinIn />
						</div>
					</a>
					<a href="https://youtube.com/channel/pit30m" class="text-gray-600 hover:text-gray-900">
						<div class="icon text-gray-600">
							<FaYoutube />
						</div>
					</a>
				</div>
			</div>
			<div class="mt-8 text-center text-gray-600">
				<p>&copy; 2023 {datasetName}. All rights reserved.</p>
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
