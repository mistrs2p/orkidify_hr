<template>
  <v-app>
    <v-container
      fluid
    >
      <Header />
      <v-form>
        <AddPhoto />        
        <Name />
        <InitialInformation :gender="gender" :years="years" :months="months" />
        <MilitaryPlan :military="military" />
        <Marriage :marriage="marriage" :majors="majors" />
        <Contact />
        <Majors :majors="majors" :years="years" />
        <ComputerSkills />
        <Accent />
        <Language />
        <Occupation :years="years" :months="months" />
        <Presenter />
        <Favorite />
        <Completion :introduction="introduction" />
        <SendBotton />
      </v-form>
    </v-container>
  </v-app>
</template>



<script>
import Header from './components/Header'
import AddPhoto from './components/AddPhoto'
import Name from './components/Name'
import InitialInformation from './components/InitialInformation'
import MilitaryPlan from './components/MilitaryPlan'
import Marriage from './components/Marriage'
import Contact from './components/Contact'
import Majors from './components/Majors'
import ComputerSkills from './components/ComputerSkills'
import Accent from './components/Accent'
import Language from './components/Language'
import Occupation from './components/Occupation'
import Presenter from './components/Presenter'
import Favorite from './components/Favorite'
import Completion from './components/Completion'
import SendBotton from './components/SendBotton'
export default {
  name: 'App',

  components: {
    Header,
    AddPhoto,
    Name,
    InitialInformation,
    MilitaryPlan,
    Marriage,
    Contact,
    Majors,
    ComputerSkills,
    Accent,
    Language,
    Occupation,
    Presenter,
    Favorite,
    Completion,
    SendBotton
  },

  data: () => ({
    gender: ['مرد', 'زن'],
    years: ['۱۳۴۰', '۱۳۴۱','۱۳۴۲','۱۳۴۳','۱۳۴۴','۱۳۴۵','۱۳۴۶','۱۳۴۷','۱۳۴۸','۱۳۴۹','۱۳۵۰','۱۳۵۱','۱۳۵۲','۱۳۵۳','۱۳۵۴','۱۳۵۵','۱۳۵۶','۱۳۵۷','۱۳۵۸','۱۳۵۹','۱۳۶۰','۱۳۶۱','۱۳۶۲','۱۳۶۳','۱۳۶۴','۱۳۶۵','۱۳۶۶','۱۳۶۷','۱۳۶۸','۱۳۶۹','۱۳۷۰','۱۳۷۱','۱۳۷۲','۱۳۷۳','۱۳۷۴','۱۳۷۵','۱۳۷۶','۱۳۷۷','۱۳۷۸','۱۳۷۹','۱۳۸۰','۱۳۸۱','۱۳۸۲','۱۳۸۳','۱۳۸۴','۱۳۸۵','۱۳۸۶','۱۳۸۷','۱۳۸۸', '۱۳۸۹','۱۳۹۰','۱۳۹۱','۱۳۹۲','۱۳۹۳','۱۳۹۴','۱۳۹۵','۱۳۹۶','۱۳۹۷','۱۳۹۸','۱۳۹۹','۱۴۰۰'],
    months: ['فروردین','اردیبهشت','خرداد','تیر','مرداد','شهریور','مهر','آبان','آذر','دی','بهمن','اسفند'],
    military: ['معافیت پزشکی','معافیت سایر','پایان طرح خدمت','در حال اتمام','در حال گذراندن','هنوز شروع نشده'],
    marriage: ['متاهل','مطلقه','مجرد'],
    majors: ['متخصص و PHD','دکترا حرفه ای','کارشناسی ارشد','کارشناسی','فوق دبپلم','دیپلم','سایر'],
    introduction: ['Linkedin Ads', 'IranTallent Ads', 'Congresses', 'Introduced By Someone', 'Heard about in the Business', 'University departments & Forums', 'Other'],
    rules: {
        required: value => !!value || 'فیلد اجباری'
    }
  }),
};
</script>

<style>
  @import './assets/style/fontface.css';
  .container {
    padding: 0;
    margin: 0
  }
  .container > .row {
    padding: 0;
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
    /* overflow: hidden; */
    flex-direction: column;
    padding: 20px 10%;
  }
  
  .row div.twoPart {
    margin: auto 4rem;
    display: flex;
    flex-wrap: wrap;
  }
  /* .row div.twoPart * {
    padding: 1rem;
  } */

  #canvas {
    border-radius: 15px;
    box-shadow: rgb(0 0 0 / 20%) 0px 10px 10px;
    border: solid 3px white;
    margin: 50px auto;
    display: block;
    background: white url(./assets/Img/Photo_Icon.png) center center no-repeat;
    cursor: pointer;
  }

  .submit {
    background: #74a55f;
    border-radius: 10px;
    color: white;
    text-align: center;
    padding: 20px 0px !important;
    display: block;
    width: 350px;
    margin: 100px auto 200px auto !important;
    cursor: pointer;
    height: auto !important;
}

</style>