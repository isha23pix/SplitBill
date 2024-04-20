<template>
    <!-- <div class="friend">
    
<ChatList/>
    </div> -->
    <!-- <v-container class="bg-primary"> -->
    <v-container >
    <v-row
      class="mb-6"
      no-gutters
    >
      <v-col :cols="cols[0]">
        <v-sheet class="pa-2 ma-2">
          .v-col-{{ cols[0] }}
        </v-sheet>
      </v-col>

      <v-col :cols="cols[1]" class="flex-grow">
        <!-- <v-sheet class="pa-2 ma-2"> -->
          <!-- .v-col-{{ cols[1] }} -->
          <!-- <ChatList/> -->
          <ChatBox/>
        <!-- </v-sheet> -->
      </v-col>
    </v-row>
  </v-container>
</template>

<script>

import { defineComponent } from "vue";
// import ChatList from "./ChatList.vue"
 import ChatBox from "./ChatBox.vue"

export default defineComponent({
  name: "FriendsComp",
  components: { 
    // ChatList,
ChatBox
 },
  computed: {
      cols() {
        const { lg, sm } = this.$vuetify.display
        return lg ? [3, 9] : sm ? [9, 3] : [6, 6]
      },
    },
});
</script>
<style>


</style>