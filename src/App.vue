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
          <div>
            <h2>ثبت تصویر</h2>
          </div>
          <canvas id="canvas"></canvas>

        </v-row>

          <h2>نام شما</h2>
        <v-row>
          <v-col
            cols="6"
          >
            <v-text-field
              label="نام (اجباری)"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-text-field
              label="Name (اجباری)"
            />
          </v-col>
          <v-col
            cols="6"
          >
            <v-text-field
              label="نام خانوادگی (اجباری)"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-text-field
              label="family (اجباری)"
            />
          </v-col>

        </v-row>

        <h2>اطلاعات اولیه</h2>
        <v-row>
          <v-col
            cols="6"
          >
            <v-select 
              label="جنسیت (اجباری)"
              :items="gender"
            />
          </v-col>
          <v-col
            cols="6"
          >
            <v-text-field
              label="نام پدر (اجباری)"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-text-field
              label=" شماره شناسنامه (اجباری)"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-text-field
              label="کد ملی (اجباری)"
            />
          </v-col>

          <v-col
            cols="3"
          >
            <v-select 
              label="سال تولد شناسنامه ای (اجباری)"
              :items="years"
            />
          </v-col>

           <v-col
            cols="6"
          >
            <v-select
              label="ماه تولد (اجباری)"
              :items="months"
            />
          </v-col>

          <v-col
            cols="3"
          >
            <v-text-field
              label="روز (اجباری))"
            />
          </v-col>

                    <v-col
            cols="3"
          >
            <v-select 
              label="سال تولد حقیقی (اجباری)"
              :items="years"
            />
          </v-col>

           <v-col
            cols="6"
          >
            <v-select
              label="ماه تولد (اجباری)"
              :items="months"
            />
          </v-col>

          <v-col
            cols="3"
          >
            <v-text-field
              label="روز (اجباری))"
            />
          </v-col>
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
    gender: ['مرد', 'زن'],
    years: ['۱۳۴۰', '۱۳۴۱','۱۳۴۲','۱۳۴۳','۱۳۴۴','۱۳۴۵','۱۳۴۶','۱۳۴۷','۱۳۴۸','۱۳۴۹','۱۳۵۰','۱۳۵۱','۱۳۵۲','۱۳۵۳','۱۳۵۴','۱۳۵۵','۱۳۵۶','۱۳۵۷','۱۳۵۸','۱۳۵۹','۱۳۶۰','۱۳۶۱','۱۳۶۲','۱۳۶۳','۱۳۶۴','۱۳۶۵','۱۳۶۶','۱۳۶۷','۱۳۶۸','۱۳۶۹','۱۳۷۰','۱۳۷۱','۱۳۷۲','۱۳۷۳','۱۳۷۴','۱۳۷۵','۱۳۷۶','۱۳۷۷','۱۳۷۸','۱۳۷۹','۱۳۸۰','۱۳۸۱','۱۳۸۲','۱۳۸۳','۱۳۸۴','۱۳۸۵','۱۳۸۶','۱۳۸۷','۱۳۸۸', '۱۳۸۹','۱۳۹۰','۱۳۹۱','۱۳۹۲','۱۳۹۳','۱۳۹۴','۱۳۹۵','۱۳۹۶','۱۳۹۷','۱۳۹۸','۱۳۹۹','۱۴۰۰'],
    months: ['فروردین','اردیبهشت','خرداد','تیر','مرداد','شهریور','مهر','آبان','آذر','دی','بهمن','اسفند']
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
  }
</style>