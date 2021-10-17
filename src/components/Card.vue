<template>
  <div>
    <v-card :loading="loading" class="mx-auto my-12" max-width="260">
      <template slot="progress">
        <v-progress-linear color="deep-purple" height="10" indeterminate></v-progress-linear>
      </template>

      <v-img height="275" :src="urlImg"></v-img>

      <v-card-title>{{name}}</v-card-title>

    </v-card>
  </div>
</template>

<script>
  export default {
    name: 'Card',
    props:['urlImg','name']
  }
</script>

<style scoped>

</style>