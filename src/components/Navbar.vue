<template>
  <div>
    <nav>
      <v-toolbar dense>
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        <v-toolbar-title>My App</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-btn text v-for="(item,index) of itemsNav" :key="index">
          {{item}}
        </v-btn>
      </v-toolbar>
    </nav>
  </div>
</template>

<script>
  export default {
    name: 'Navbar',
    data() {
      return {
        itemsNav: ['Inicio', 'Buscar', 'Acerca de']
      }
    },
  }
</script>