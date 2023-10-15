<script>
  export let expand
  export let dir
</script>
<div  class={`max-sm:relative absolute  bg-white md:right-6 rounded-xl shadow-xl max-sm:shadow-none max-sm:my-2 max-sm:top-[5px] top-10 h-0 transition-all duration-500 overflow-hidden ${dir ? "right-0" : ""}  ${expand ? "h-[100px] " : "p-0"}`}>
 <div>history</div>
<div>our team</div>
<div>blog</div>   
</div>
<style>
    div > div {
        width: 100px;
        padding:2px 15px;
        cursor: pointer;
        text-transform: capitalize;
    }
</style>