<template>
  <v-container fluid>
    <v-row no-gutters>
      <v-col :cols="showLeftPanel ? 4 : 0" v-if="showLeftPanel">
        <div class="left-panel">
          <v-card variant="flat" :elevation="0" color="transparent">
            <v-toolbar class="tool" color="rgba(208, 195, 210, 0.848)" dense flat>
            <v-row class="fill-height" no-gutters align="center">
              <v-col cols="5" class="px-0">
                <v-text-field
                  hide-details
                  outlined
                  dense
                  solo
                  color="transparent"
                  placeholder="Search"
                  rounded
                  clearable
                  append-inner-icon="mdi-magnify"
                 
                ></v-text-field>
              </v-col>
              <v-col cols="7">
                <v-btn variant="outlined" class="expense" style="border: 3px solid #673ab7; margin-right: 8px;">
                  <span class="label"  style="color: #673ab7;"><b>+ Add Friend</b></span>
                </v-btn>
                <v-btn :class="notificationIcon" icon >
                  <v-icon class="icon">mdi-bell-outline</v-icon>
                </v-btn>
              </v-col>
            </v-row>
          </v-toolbar>
      </v-card>
      <ContactList @chat-selected="handleChatSelected"/>
        </div>
      </v-col>

      <v-col :cols="showLeftPanel ? 8 : 12">
        <div class="right-panel">
          <ChatBox :chat="selectedChat"/>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import ContactList from './ContactList.vue';
import ChatBox from './ChatBox.vue';
export default {
  name: "FriendsMain",
  components: {
    ContactList,
    ChatBox
  },
  data: () => ({
    showLeftPanel: true, // Initially show 
  }),
  mounted() {
    this.handleResize();
    window.addEventListener('resize', this.handleResize);
  },
  beforeUnmount() {
    window.removeEventListener('resize', this.handleResize);
  },
  methods: {
    handleResize() {
      const smBreakpoint = 960; //width for 'sm' in Vuetify
      this.showLeftPanel = window.innerWidth >= smBreakpoint;
    },
    handleChatSelected(chat) {
      this.selectedChat = chat;
    }
  },
}
</script>

<style scoped>
.left-panel, .right-panel {
  padding: 16px;
}
.left-panel{
  background-color: transparent;
}
.tool{  
  box-shadow: none;
  border:0px;
}
.v-card{
  background-color: rgba(208, 195, 210, 0.848) ;
  box-shadow: none;
}
.icon {
    color:#673ab7;
    }
    .notificationIcon:active {
    color: #673ab7;
    }
</style>
