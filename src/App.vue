<template>
  <v-app>
    <v-container
      fluid
      class="topImg"
    >
      <Header />
      <v-form>
        <AddPhoto />        
        <Name />
        <InitialInformation :gender="gender" :years="years" :months="months" />
        <h2>طرح و سربازی</h2>
        <v-row>
          <v-col
            cols="6"
          >
            <v-select 
              label="وضعیت سربازی"
              :items="military"
            />
          </v-col>
          <v-col
            cols="6"
          >
            <v-text-field 
              label="علت معافیت"
            />
          </v-col>
        </v-row>

        <h2>وضعیت تاهل</h2>
        <v-row>
          <v-col
            cols="6"
          >
            <v-select 
              label="وضعیت تاهل"
              :items="marriage"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-select 
              label="تحصیلات همسر"
              :items="majors"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-text-field
              label="شغل همسر"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-text-field
              label="تعداد فرزندان"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-text-field
              label="افراد تحت تکفل"
            />
          </v-col>
        </v-row>

        <h2>اطلاعات تماس</h2>
        <v-row>
           <v-col
            cols="6"
          >
            <v-text-field
              label="تلفن (اجباری)"
            />
          </v-col>
          
           <v-col
            cols="6"
          >
            <v-text-field
              label="موبایل"
            />
          </v-col>

           <v-col
            cols="6"
          >
            <v-text-field
              label="ایمیل (اجباری)"
            />
          </v-col>

           <v-col
            cols="6"
          >
            <v-text-field
              label="شهر (اجباری)"
            />
          </v-col>

           <v-col
            cols="12"
          >
            <v-text-field
              label="آدرس (اجباری)"
            />
          </v-col>
        </v-row>

        <h2>مقطع تحصیلی (لطفا از آخرین مقطع تحصیلی شروع کنید)</h2>
        <v-row>
           <v-col
            cols="6"
          >
            <v-text-field
              label="رشته تحصیلی (اجباری)"
            />
          </v-col>
          
           <v-col
            cols="6"
          >
            <v-select
              label="مقطع تحصیلی (اجباری)"
              :items="majors"
            />
          </v-col>

           <v-col
            cols="6"
          >
            <v-text-field
              label="نام دانشگاه (اجباری)"
            />
          </v-col>

           <v-col
            cols="3"
          >
            <v-select
              label="سال ورود (اجباری)"
              :items="years"
            />
          </v-col>

           <v-col
            cols="3"
          >
            <v-select
              label="سال خروج (اجباری)"
              :items="years"
            />
          </v-col>
          <v-divider />
          <v-col
            cols="6"
          >
            <v-text-field
              label="رشته تحصیلی"
            />
          </v-col>
          
           <v-col
            cols="6"
          >
            <v-select
              label="مقطع تحصیلی"
              :items="majors"
            />
          </v-col>

           <v-col
            cols="6"
          >
            <v-text-field
              label="نام دانشگاه"
            />
          </v-col>

           <v-col
            cols="3"
          >
            <v-select
              label="سال ورود"
              :items="years"
            />
          </v-col>

           <v-col
            cols="3"
          >
            <v-select
              label="سال خروج"
              :items="years"
            />
          </v-col>
          <v-divider />
          <v-col
            cols="6"
          >
            <v-text-field
              label="رشته تحصیلی"
            />
          </v-col>
          
           <v-col
            cols="6"
          >
            <v-select
              label="مقطع تحصیلی"
              :items="majors"
            />
          </v-col>

           <v-col
            cols="6"
          >
            <v-text-field
              label="نام دانشگاه"
            />
          </v-col>

           <v-col
            cols="3"
          >
            <v-select
              label="سال ورود"
              :items="years"
            />
          </v-col>

           <v-col
            cols="3"
          >
            <v-select
              label="سال خروج"
              :items="years"
            />
          </v-col>
        </v-row>

        <h2>Computer Skills</h2>
        
        <v-row>
          <v-col
            cols="4"
          >
            <v-checkbox
              label="Word"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="Outlook"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="Excel"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="Medical Search"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="Power Point"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="Fast Typing"
            />
          </v-col>

          <v-col
            cols="12"
          >
            <v-text-field
              label="آیا با مهارت کامپیوتری دیگری آشنایی دارید؟"
            />
          </v-col>
        </v-row>

        <h2>آشنایی با لهجه های محلی</h2>

        <v-row>
          <v-col
            cols="6"
          >
            <v-checkbox
              label="کردی"
            />
          </v-col>

          <v-col
            cols="6"
          >
            <v-checkbox
              label="ترکی"
            />
          </v-col>

           <v-col
            cols="12"
          >
            <v-text-field
              label="آیا با گویش های دیگری آشنایی دارید؟"
            />
          </v-col>
        </v-row>


        <h2>زبان های خارجی</h2>
        <v-row>
          <v-col
            cols="4"
          >
            <v-checkbox
              label="IELTS"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="TOEFL"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="GRE"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="English Intermediate"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="English Beginner"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="French Advanced"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="French Intermediate"
            />
          </v-col>

          <v-col
            cols="4"
          >
            <v-checkbox
              label="French Beginner"
            />
          </v-col>

          <v-col
            cols="12"
          >
            <v-text-field
              label="آیا با زبان خارجی دیگری آشنایی دارید؟"
            />
          </v-col>
        </v-row>

        <h2>سوابق شغلی</h2>
        <v-row>
          <v-col
            cols="6"
          >
            <v-text-field 
              label="عنوان شغلی (اجباری)"
            />
          </v-col>
          
          <v-col
            cols="6"
          >
            <v-text-field 
              label="نام شرکت (اجباری)"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="ماه ورود (اجباری)"
              :items="months"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="سال ورود (اجباری)"
              :items="years"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="ماه خروج (اجباری)"
              :items="months"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="سال خروج (اجباری)"
              :items="years"
            />
          </v-col>
          <v-col
            cols="12"
          >
            <v-text-field 
              label="علت تغییر (اجباری)"
            />
          </v-col>

          <v-divider></v-divider>

          <v-col
            cols="6"
          >
            <v-text-field 
              label="عنوان شغلی"
            />
          </v-col>
          
          <v-col
            cols="6"
          >
            <v-text-field 
              label="نام شرکت"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="ماه ورود"
              :items="months"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="سال ورود"
              :items="years"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="ماه خروج"
              :items="months"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="سال خروج"
              :items="years"
            />
          </v-col>
          <v-col
            cols="12"
          >
            <v-text-field 
              label="علت تغییر"
            />
          </v-col>

          <v-divider></v-divider>

          <v-col
            cols="6"
          >
            <v-text-field 
              label="عنوان شغلی"
            />
          </v-col>
          
          <v-col
            cols="6"
          >
            <v-text-field 
              label="نام شرکت"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="ماه ورود"
              :items="months"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="سال ورود"
              :items="years"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="ماه خروج"
              :items="months"
            />
          </v-col>
          <v-col
            cols="3"
          >
            <v-select 
              label="سال خروج"
              :items="years"
            />
          </v-col>
          <v-col
            cols="12"
          >
            <v-text-field 
              label="علت تغییر"
            />
          </v-col>
        </v-row>
        
        <h2>معرف</h2>
        <v-row>
          <v-col
            cols="6"
          >
            <v-text-field
              label="نام معرف"
            />

          </v-col>

          <v-col
            cols="3"
          >
            <v-text-field
              label="عنوان شغلی"
            />

          </v-col>

          <v-col
            cols="3"
          >
            <v-text-field
              label="محل فعالیت"
            />

          </v-col>

          <v-divider></v-divider>

          <v-col
            cols="6"
          >
            <v-text-field
              label="نام معرف"
            />

          </v-col>

          <v-col
            cols="3"
          >
            <v-text-field
              label="عنوان شغلی"
            />

          </v-col>

          <v-col
            cols="3"
          >
            <v-text-field
              label="محل فعالیت"
            />

          </v-col>
        </v-row>

        <v-row>
          <v-col
            cols="3"
          >
            <v-checkbox
              label="مارکتینگ علمی"
            />
          </v-col>

          <v-col
            cols="3"
          >
            <v-checkbox
              label="مدیکال انفورماتیک"
            />
          </v-col>

          <v-col
            cols="3"
          >
            <v-checkbox
              label="فناوری اطلاعات"
            />
          </v-col>

          <v-col
            cols="3"
          >
            <v-checkbox
              label="پشتیبانی بیماران"
            />
          </v-col>

          <v-col
            cols="3"
          >
            <v-checkbox
              label="منابع انسانی"
            />
          </v-col>
        </v-row>

        <h2>سوالات تکمیلی</h2>
        <v-row>
          <v-col
            cols="12"
          >
            <v-text-field 
              label="نحوه آشنایی با ارکید فارمد"
            />
          </v-col>

          <v-col
            cols="12"
          >
            <v-text-field 
              label="حقوق پیشنهادی شما (اجباری)"
            />
          </v-col>

          <v-col
            cols="12"
          >
            <v-text-field 
              label="سابقه جراحی - بیماری"
            />
          </v-col>

          <v-col
            cols="12"
          >
            <v-text-field 
              label="آیا در شرکت های همکار یا رقیب ارکید فارمد کسی را می شناسید؟ اگر بله با ایشان چه نسبتی دارید؟ (اجباری)"
            />
          </v-col>

          <v-col
            cols="12"
          >
            <v-text-field 
              label="توضیحات تکمیلی که لازم می دانید در مورد شما بدانیم"
            />
          </v-col>
        </v-row>
        <v-row>
          <v-col
            cols="12"
          >
            <div class="submit">ارسال فرم</div>
          </v-col>
        </v-row>
      </v-form>
    </v-container>
  </v-app>
</template>



<script>
import Header from './components/Header'
import AddPhoto from './components/AddPhoto'
import Name from './components/Name'
import InitialInformation from './components/InitialInformation'
export default {
  name: 'App',

  components: {
    Header,
    AddPhoto,
    Name,
    InitialInformation,

  },

  data: () => ({
    gender: ['مرد', 'زن'],
    years: ['۱۳۴۰', '۱۳۴۱','۱۳۴۲','۱۳۴۳','۱۳۴۴','۱۳۴۵','۱۳۴۶','۱۳۴۷','۱۳۴۸','۱۳۴۹','۱۳۵۰','۱۳۵۱','۱۳۵۲','۱۳۵۳','۱۳۵۴','۱۳۵۵','۱۳۵۶','۱۳۵۷','۱۳۵۸','۱۳۵۹','۱۳۶۰','۱۳۶۱','۱۳۶۲','۱۳۶۳','۱۳۶۴','۱۳۶۵','۱۳۶۶','۱۳۶۷','۱۳۶۸','۱۳۶۹','۱۳۷۰','۱۳۷۱','۱۳۷۲','۱۳۷۳','۱۳۷۴','۱۳۷۵','۱۳۷۶','۱۳۷۷','۱۳۷۸','۱۳۷۹','۱۳۸۰','۱۳۸۱','۱۳۸۲','۱۳۸۳','۱۳۸۴','۱۳۸۵','۱۳۸۶','۱۳۸۷','۱۳۸۸', '۱۳۸۹','۱۳۹۰','۱۳۹۱','۱۳۹۲','۱۳۹۳','۱۳۹۴','۱۳۹۵','۱۳۹۶','۱۳۹۷','۱۳۹۸','۱۳۹۹','۱۴۰۰'],
    months: ['فروردین','اردیبهشت','خرداد','تیر','مرداد','شهریور','مهر','آبان','آذر','دی','بهمن','اسفند'],
    military: ['معافیت پزشکی','معافیت سایر','پایان طرح خدمت','در حال اتمام','در حال گذراندن','هنوز شروع نشده'],
    marriage: ['متاهل','مطلقه','مجرد'],
    majors: ['متخصص و PHD','دکترا حرفه ای','کارشناسی ارشد','کارشناسی','فوق دبپلم','دیپلم','سایر']
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
    /* overflow: hidden; */
    flex-direction: column;
    margin: auto 4rem;
  }
  
  .row div.twoPart {
    display: flex;
    flex-wrap: wrap;
  }
  .row div.twoPart * {
    /* padding: 1rem; */
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