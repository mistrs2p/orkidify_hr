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
        <v-row class="addPhoto">
          <h2>ثبت تصویر</h2>
          <canvas id="canvas"></canvas>

        </v-row>
            
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
    margin: 0
  }
  h1 {
    color: #004b70;
    font-size: 25px;
    line-height: 1;
  }
  h2 {
    color: #c1ced9;
    margin: 0px 15px;
  }
  .welcomeText {
    color: #a0a0a0;
    font-size: 15px;
    margin-bottom: 40px;
  }
  .row {
    background: linear-gradient(180deg, #f1f5f8 0%, #ffffff 100%);
    overflow: hidden;
  }

  #canvas {
    border-radius: 15px;
    box-shadow: rgb(0 0 0 / 20%) 0px 10px 10px;
    border: solid 3px white;
    margin: 50px auto;
    display: block;
    background: white url(./assets/Img/Photo_Icon.png) center center no-repeat;
    cursor: pointer;
  }

  .addPhoto {
    flex-direction: column
  }
</style>