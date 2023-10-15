<script>
	export let title 
    export let showlist=false
    
</script>

<div class={`relative z-20`}>
    <!-- svelte-ignore a11y-no-static-element-interactions -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <div class="flex items-center gap-2 mx-10 max-sm:mx-0 cursor-pointer justify-center max-sm:justify-start" on:click>
         <p class={`capitalize ${showlist ? "text-black " : "text-gray-500"} `}>{title}</p>
         <img src={`${showlist ? "/icons/icon-arrow-up.svg" : "/icons/icon-arrow-down.svg"} `} alt="">
    </div>
   
   <slot />
</div>