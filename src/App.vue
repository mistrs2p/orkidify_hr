<template>
  <v-app>
    <v-container
      fluid
      class="topImg"
    >
      <v-row>
        <v-col>
          <v-img
            min-height="416"
            src="./assets/Img/Header_small.png"

          >
          </v-img>
          <h1
            class="text-center"  
          >به ارکید فارمد خوش آمدید</h1>
          <p class="welcomeText text-center">لطفا اطلاعات فرم زیر را با دقت تکمیل نمایید</p>
        </v-col>
      </v-row>
      <v-form>
            
      </v-form>
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
  h1 {
    color: #004b70;
    font-size: 25px;
    line-height: 1;
  }
  .welcomeText {
    color: #a0a0a0;
    font-size: 15px;
    margin-bottom: 40px;
  }
</style>