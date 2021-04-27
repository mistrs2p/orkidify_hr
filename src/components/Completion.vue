<template>
    <v-row>
        <div class="twoPart">
            <h2>سوالات تکمیلی</h2>
        </div>
        <div class="twoPart">
            <v-col
            cols="12"
            >
            <v-select 
                label="نحوه آشنایی با ارکید فارمد"
                :items="introduction"
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
        </div>
    </v-row>
</template>

<script>
export default {
    props: ['introduction']
}
</script>

<style>

</style>