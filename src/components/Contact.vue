<template>
  <v-row>
    <div class="twoPart">
      <h2>اطلاعات تماس</h2>
    </div>
    <div class="twoPart">
      <v-col
        cols="6"
      >
        <v-text-field
          :rules="[rules.required]"
          label="تلفن (اجباری)"
        />
      </v-col>
      
        <v-col
        cols="6"
      >
        <v-text-field
          :rules="[rules.required]"
          label="موبایل"
        />
      </v-col>

        <v-col
        cols="6"
      >
        <v-text-field
          :rules="[rules.required]"
          label="ایمیل (اجباری)"
        />
      </v-col>

        <v-col
        cols="6"
      >
        <v-text-field
          :rules="[rules.required]"
          label="شهر (اجباری)"
        />
      </v-col>

        <v-col
        cols="12"
      >
        <v-text-field
          :rules="[rules.required]"
          label="آدرس (اجباری)"
        />
      </v-col>
    </div>
  </v-row>
</template>

<script>
export default {
  props: ['rules']
}
</script>

<style>

</style>