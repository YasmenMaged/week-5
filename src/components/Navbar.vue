<template>
  <nav>
    <v-app-bar flat app dark>
      <v-app-bar-nav-icon class="grey--text" @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title class="text-uppercase white--text">
        <span>Navbar</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-export</v-icon>
      </v-btn>
    </v-app-bar>
    
    
    <v-navigation-drawer v-model="drawer" app dark class="white--text">
      <v-flex class="mt-5">
      <Popup/>
    </v-flex>

      <p>item1</p>
      <p>item2</p>
    </v-navigation-drawer>
    
  </nav>
</template>

<script>
import Popup from './Popup.vue'
export default {
  components:{
    Popup
  },
  data(){
    return{
      drawer: false
    }
  }
};
</script>
