<script>
export let showMenu;
import CompanyList from "./CompanyList.svelte";
import DropDown from "./DropDown.svelte";
import FeaturesList from "./FeaturesList.svelte";
    let showFeatures=false
    let showCompany=false


    const toggleShowFeatures=()=>{
        showFeatures=!showFeatures;
}
const toggleShowCompany=()=>{
        showCompany=!showCompany;
}
const togleMenu=()=>{
    showMenu=!showMenu;

}
</script>

<div class={`fixed transition-all z-20 duration-500 overflow-hidden right-0 h-[100%] bg-[rgba(0,0,0,0.3)] top-0 ${showMenu ? "w-[100%]" : "w-0"}`}>
   
<div class="w-[70%] h-[100%] absolute bg-white right-0">
    <div class="flex justify-end p-2 mt-3">
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
        <img src="/icons/icon-close-menu.svg" alt="" on:click>
    </div>
    <div class="flex justify-between  flex-col py-2 px-8 w-[80%] ">
        <DropDown title="feature" on:click={toggleShowFeatures} showlist={showFeatures}>
          <FeaturesList expand={showFeatures} dir={false}/>
        </DropDown>
        <DropDown title="Company" on:click={toggleShowCompany} showlist={showCompany}>
         <CompanyList expand={showCompany} dir={false}/>
        </DropDown>
        <div class="capitalize cursor-pointer text-gray-500 my-2 hover:text-black">
          careers
        </div>
        <div class="capitalize cursor-pointer text-gray-500 my-2 hover:text-black">
  
          about
        </div>
      
    </div>  
    <div class="mt-2 mx-auto w-1/2">
        <div class="py-2 px-4 text-gray-500 text-center hover:text-black cursor-pointer">login</div>
        <div class="py-2 px-4 rounded-lg  text-gray-500 text-center hover:text-black hover:border cursor-pointer">Register</div>
        </div>
</div>
</div>