<script>
	import NavBar from "../components/NavBar.svelte";


</script>

<main >
<NavBar />
<section class="w-[80%] mx-auto flex justify-between items-center my-10 relative z-10 max-sm:w-[100%] max-sm:flex-col-reverse ">
<div class="w-1/2 max-sm:w-full max-sm:flex max-sm:flex-col max-sm:items-center px-3">
<div class="max-sm:flex gap-2 max-sm:my-3">
    <h1 class="text-7xl font-bold max-sm:text-4xl">make</h1>
<h1  class="text-7xl font-bold max-sm:text-4xl">remote work</h1>
</div>
    
<p class="text-sm text-gray-600 mt-16 capitalize">Lorem ipsum dolor sit amet consectetur adipisicing elit. 
    Hic beatae aut saepe deleniti? Sed obcaecati vitae possimus,
     officia accusantium expedita unde nobis enim exercitationem labore 
     in at beatae ex ipsum!</p>
     <button class="px-5 py-2 rounded-xl text-white font-bold bg-black mt-9">
        learn more
     </button>
     <div class="flex justify-between items-center mt-36">
       <img src="/icons/client-databiz.svg" alt="">
       <img src="/icons/client-audiophile.svg" alt="">
       <img src="/icons/client-meet.svg" alt="">
       <img src="/icons/client-maker.svg" alt="">
     </div>
</div>
<div class="w-1/2 h-[100%] max-sm:w-full">
<img src="/icons/image-hero-desktop.png" alt="" class="object-contain md:aspect-square">
</div>
</section>
</main>
