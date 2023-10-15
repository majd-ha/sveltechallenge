<script>
    export let expand;
    export let dir;
</script> 
 
 <div class={`absolute bg-white w-fit max-sm:relative rounded-xl max-sm:-left-[10px] right-5 top-10 z-20 max-sm:shadow-none shadow-xl max-sm:top-[0px] h-0 transition-hieght duration-500 overflow-hidden px-6 max-sm:my-2 ${dir ? " max-sm:-left-[20px]" : ""}  ${expand ? "h-[180px] " : "p-0"}`}>


    <div class="listItem">
        <img src="/icons/icon-todo.svg" alt=""   width="20" height="20"/>
        <p >todo list</p>
      </div>
      <div class="listItem">
        <img src="/icons/icon-calendar.svg" alt="" width="20" height="20" />
        <p>calender</p>
      </div>
      <div class="listItem">
        <img src="/icons/icon-reminders.svg" alt="" width="20" height="20" />
        <p>reminders</p>
      </div>
      <div class="listItem">
        <img src="/icons/icon-planning.svg" alt="" width="20" height="20" />
        <p>planing</p>
      </div>
    </div>