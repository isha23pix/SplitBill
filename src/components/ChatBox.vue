<template>
    <div class="chatList">

    </div>

</template>
<script>
import { defineComponent } from "vue";
 

   export default defineComponent({
     name: "ChatBox",
  
   });
</script>
<style>
.chatList{
    background-color: aquamarine;
    justify-content: flex-start;
    display: flex;
    flex-direction: column;
    border-radius: var(--br-6xl);
    box-shadow: 0px 4px 5px 2px rgba(121, 197, 239, 0.38);
    background-color: var(--color-white);
    box-sizing: border-box;
    /* height:auto; */
    height: 635px;
}
</style>