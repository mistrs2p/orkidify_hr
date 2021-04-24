<template>
  <v-app>
  <v-container
    fluid
    class="topImg"
  >
    <v-col>
      <v-img
        min-height="416"
        src="./assets/Img/Header_small.png"

      >
      </v-img>
    
    </v-col>
  </v-container>

  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {
  },

  data: () => ({
    //
  }),
};
</script>

<style>
  @import './assets/style/fontface.css';
  .topImg * {
    padding: 0;
  }
</style>