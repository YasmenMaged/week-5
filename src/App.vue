<template>
  <v-app class="grey ligten-4">
    <Navbar></Navbar>
    <v-main>
      <router-view/>
      <Table></Table>

      </v-main> 
   

    
    
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Table from '@/components/Table.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Table
  },
  data: () => ({
    //
  }),
};
</script>
