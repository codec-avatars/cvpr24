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
	import { get_root_for_style } from 'svelte/internal';
  
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
		<NavLi href="{base}/#overview">Overview</NavLi>
		<NavLi href="{base}/#schedule">Schedule</NavLi>
		<NavLi href="{base}/#speakers">Speakers</NavLi>
		<NavLi href="{base}/#organizers">Organizers</NavLi>
	</NavUl>
</Navbar>


<body>
<!-- Background image 1 from https://unsplash.com/photos/F6Kj8ovnUvM -->
<!-- Background image 2 from https://unsplash.com/photos/yLcPSvJkGrM -->
<!-- <section class="bg-cover bg-center h-96 relative" style="background-image: url('hero_bg.jpg')"> -->

<section class="bg-white dark:bg-gray-900">
    <div class="py-8 px-4 mx-auto max-w-screen-xl text-center lg:py-16 lg:px-12">
        
        <h1 class="mb-4 text-4xl font-extrabold tracking-tight leading-none text-gray-900 md:text-5xl lg:text-6xl dark:text-white">
			Social Presence with Codec Avatars
		</h1>
        <p class="mb-8 text-lg font-normal text-gray-500 lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
			Full-day CVPR'24 workshop on Tuesday, June 18, 2024 <br />
			Summit 333, at the Seattle Convention Center
		</p>
    </div>
</section>

<section class="container mx-auto px-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white" id="overview"><a href="{base}/#overview">Overview</a></h2>
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
		<h2 class="text-4xl font-extrabold dark:text-white" id="schedule"><a href="{base}/#schedule">Schedule</a></h2>
		
		
		<div class="py-4">
		<div class="relative overflow-x-auto shadow-md sm:rounded-lg">
			<table class="w-full text-sm text-left rtl:text-right text-gray-500 dark:text-gray-400">
				<thead class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400">
					<tr>
						<th scope="col" class="px-6 py-3">
							Time
						</th>
						<th scope="col" class="px-6 py-3">
							Speaker
						</th>
						<th scope="col" class="px-6 py-3">
							Topic
						</th>
					</tr>
				</thead>
				<tbody>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							9:00 - 10:15
						</th>
						<td class="px-6 py-4">
							TBD
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							10:15 - 10:30
						</th>
						<td class="px-6 py-4">
							☕
						</td>
						<td class="px-6 py-4">
							15 min break
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							10:30 - 11:15
						</th>
						<td class="px-6 py-4">
							Prof. Christian Theobalt
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							11:15 - 12:00
						</th>
						<td class="px-6 py-4">
							Prof. Yaser Sheikh
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							12:00 - 1:00
						</th>
						<td class="px-6 py-4">
							🥪
						</td>
						<td class="px-6 py-4">
							Lunch break
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							1:00 - 1:45
						</th>
						<td class="px-6 py-4">
							TBD
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							1:45 - 2:30
						</th>
						<td class="px-6 py-4">
							TBD
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							2:30 - 3:15
						</th>
						<td class="px-6 py-4">
							Prof. Michael Black
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							3:15 - 3:30
						</th>
						<td class="px-6 py-4">
							☕
						</td>
						<td class="px-6 py-4">
							15 min break
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							3:30 - 4:15
						</th>
						<td class="px-6 py-4">
							Prof. Angela Dai
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
					<tr class="odd:bg-white odd:dark:bg-gray-900 even:bg-gray-50 even:dark:bg-gray-800 border-b dark:border-gray-700">
						<th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap dark:text-white">
							4:15 - 5:00
						</th>
						<td class="px-6 py-4">
							TBD
						</td>
						<td class="px-6 py-4">
							TBD
						</td>
					</tr>
				</tbody>
			</table>
		</div>


	</div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white" id="speakers"><a href="{base}/#speakers">Keynote Speakers</a></h2>

		<div class="grid md:grid-cols-4 gap-4">
			
			<div class="grid gap-4">
				<div class="py-4 max-w-sm rounded overflow-hidden shadow-lg">
					<a href="https://www.professoren.tum.de/en/dai-angela/">
						<img class="w-full aspect-square object-cover object-top" src="Dai_Angela.jpg" alt="Prof. Kanazawa">
					</a>
					<div class="px-6 py-4">
					<div class="font-bold text-xl mb-2"><a href="https://people.eecs.berkeley.edu/~kanazawa/">Prof. Angela Dai</a></div>
					<p class="text-gray-700 text-base">
						Assistant Professor at the Technical University of Munich where she leads the 3D AI lab.
						Her research has been recognized through an ERC Starting Grant, Eurographics Young Researcher Award, Google Research Scholar Award, ZDB Junior Research Group Award, an ACM SIGGRAPH Outstanding Doctoral Dissertation Honorable Mention, as well as a Stanford Graduate Fellowship.
					</p>
					</div>
				</div>
			</div>

			<div class="grid gap-4">
				<div class="py-4 max-w-sm rounded overflow-hidden shadow-lg">
					<a href="https://ps.is.mpg.de/person/black">
						<img class="w-full aspect-square object-cover object-top" src="mjb_photo.jpg" alt="Prof. Kanazawa">
					</a>
					<div class="px-6 py-4">
					<div class="font-bold text-xl mb-2"><a href="https://ps.is.mpg.de/person/black">Prof. Michael Black</a></div>
					<p class="text-gray-700 text-base">
						Honorarprofessor at the University of Tübingen and one of the founding directors at the Max Planck Institute for Intelligent Systems in Tübingen, 
						Germany, where he leads the Perceiving Systems department and serves as Managing Director.
					</p>
					</div>
				</div>
			</div>


			<div class="grid gap-4">
				<div class="py-4 max-w-sm rounded overflow-hidden shadow-lg">
					<a href="https://people.mpi-inf.mpg.de/~theobalt/">
						<img class="w-full aspect-square object-cover object-top" src="theobalt_photo.jpg" alt="Prof. Kanazawa">
					</a>
					<div class="px-6 py-4">
					<div class="font-bold text-xl mb-2"><a href="https://people.mpi-inf.mpg.de/~theobalt/">Prof. Christian Theobalt</a></div>
					<p class="text-gray-700 text-base">
						Director of the Visual Computing and AI Department at MPI for Informatics. Professor of Computer Science at Saarland University,
						and Director of the Saarbruecken Center for Visual Computing, Interaction and Artificial Intelligence.
					</p>
					</div>
				</div>
			</div>
			
			<div class="grid gap-4">
				<div class="py-4 max-w-sm rounded overflow-hidden shadow-lg">
					<a href="https://www.cs.cmu.edu/~yaser/">
						<img class="w-full aspect-square object-cover object-top" src="yaser_photo.jpg" alt="Prof. Kanazawa">
					</a>
					<div class="px-6 py-4">
					<div class="font-bold text-xl mb-2"><a href="https://www.cs.cmu.edu/~yaser/">Prof. Yaser Sheikh</a></div>
					<p class="text-gray-700 text-base">
						Vice President and founding director of the Meta Reality Lab in Pittsburgh, devoted to achieving
						photorealistic social interactions in augmented and virtual reality. He is a consulting professor at the Robotics Institute, Carnegie Mellon University.
					</p>
					</div>
				</div>
			</div>

		</div>

	</div>
</section>

<section class="container mx-auto px-4 py-4">
	<div class="grid">
		<h2 class="text-4xl font-extrabold dark:text-white " id="organizers"><a href="{base}/#organizers">Organizers</a></h2>

		
		<div class="grid grid-cols-4 md:grid-cols-4 gap-8 py-6 ">
			
			<div class="grid gap-4">
				<a href="https://una-dinosauria.github.io">
				<div class="flex items-center space-x-4 rtl:space-x-reverse">
					<div class="flex-shrink-0">
					   <img class="w-8 h-8 rounded-full" src="citations.jfif" alt="Neil image">
					</div>
					<div class="flex-1 min-w-0">
					   <p class="text-sm font-medium text-gray-900 truncate dark:text-white">
						  Julieta Martinez
					   </p>
					   <p class="text-sm text-gray-500 truncate dark:text-gray-400">
						  Research Scientist at Meta
					   </p>
					</div>
				 </div>
				</a>
			</div>

			<div class="grid gap-4">
				<a href="https://ps.is.mpg.de/person/jromero">
				<div class="flex items-center space-x-4 rtl:space-x-reverse">
					<div class="flex-shrink-0">
					   <img class="w-8 h-8 rounded-full" src="jr.jfif" alt="Neil image">
					</div>
					<div class="flex-1 min-w-0">
					   <p class="text-sm font-medium text-gray-900 truncate dark:text-white">
						  Javier Romero
					   </p>
					   <p class="text-sm text-gray-500 truncate dark:text-gray-400">
						  Research Scientist at Meta
					   </p>
					</div>
				 </div>
				</a>
			</div>
			
			
			<div class="grid gap-4">
				<a href="https://zollhoefer.com/">
				<div class="flex items-center space-x-4 rtl:space-x-reverse">
					<div class="flex-shrink-0">
					   <img class="w-8 h-8 rounded-full" src="mz.jfif" alt="Neil image">
					</div>
					<div class="flex-1 min-w-0">
					   <p class="text-sm font-medium text-gray-900 truncate dark:text-white">
						  Michael Zollhoefer
					   </p>
					   <p class="text-sm text-gray-500 truncate dark:text-gray-400">
						  Research Director at Meta
					   </p>
					</div>
				 </div>
				 </a>
			</div>
			
			<div class="grid gap-4">
				<a href="http://www.cs.cmu.edu/~yaser">
				<div class="flex items-center space-x-4 rtl:space-x-reverse">
					<div class="flex-shrink-0">
					   <img class="w-8 h-8 rounded-full" src="ys.jfif" alt="Neil image">
					</div>
					<div class="flex-1 min-w-0">
					   <p class="text-sm font-medium text-gray-900 truncate dark:text-white">
						  Yaser Sheikh
					   </p>
					   <p class="text-sm text-gray-500 truncate dark:text-gray-400">
						  Research VP at Meta
					   </p>
					</div>
				 </div>
				</a>
			</div>


		</div>

	</div>
</section>

</body>


<footer class="bg-gray-200 py-8 mt-8">
	<div class="container mx-auto px-4">
		<div class="flex justify-between items-center">

			<div class="text-gray-600">
				<p>
					Contact: <a href="mailto:julietamartinez@meta.com" class="hover:text-gray-900">julietamartinez@meta.com</a>
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
