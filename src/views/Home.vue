<template>
  <div>
    <Navbar />

    <v-container>
      <v-row no-gutters>
        <v-col cols="12" sm="6" lg="4" v-for="(item,index) of getPersonajes" :key="index">
          <Card :urlImg="item.imagen" :name="item.nombre" />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
  import {
    mapGetters
  } from 'vuex'
  import Navbar from '@/components/Navbar.vue'
  import Card from '@/components/Card.vue'

  export default {
    name: 'Home',
    components: {
      Navbar,
      Card
    },
    computed: {
      ...mapGetters(['getPersonajes'])
    }
  }
</script>