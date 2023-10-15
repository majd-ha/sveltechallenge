<script>
    import SideMenu from '../components/SideMenu.svelte';
    import CompanyList from "./CompanyList.svelte";
    import DropDown from "./DropDown.svelte";
    import FeaturesList from "./FeaturesList.svelte";
    let showFeatures=false
    let showCompany=false
    let showMenu=false

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

<nav class="flex justify-between p-2 py-4 items-start max-sm:items-center">
     
   <div class="flex justify-between w-[40%] max-sm:justify-start">

  
    <div class="w-[20%] max-sm:w-[60%] px-3 py-2">
    <img src= '/icons/logo.svg' alt=""/>
    </div>
    <div class="flex justify-between items-start px-5 w-[80%] max-sm:hidden">
      <DropDown title="feature" on:click={toggleShowFeatures} showlist={showFeatures}>
        <FeaturesList expand={showFeatures} dir={true}/>
      </DropDown>
      <DropDown title="Company" on:click={toggleShowCompany} showlist={showCompany}>
       <CompanyList expand={showCompany} dir={false}/>
      </DropDown>
      <div class="capitalize cursor-pointer text-gray-500 px-10  hover:text-black">
        careers
      </div>
      <div class="capitalize cursor-pointer text-gray-500 px-10  hover:text-black">

        about
      </div>
    
    </div>  
</div>
    <div class="flex justify-between items-start mr-5 max-sm:hidden">
      <div class="py-1 px-4 text-gray-500 hover:text-black cursor-pointer">login</div>
      <div class="py-1 px-4 rounded-lg  text-gray-500 hover:text-black cursor-pointer hover:border">Register</div>
      </div>
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <!-- svelte-ignore a11y-no-static-element-interactions -->
      <div class="hidden max-sm:block" on:click={togleMenu}>
        <img src="/icons/icon-menu.svg" alt="">
      </div>
</nav>
<SideMenu showMenu={showMenu} on:click={togleMenu}/>

