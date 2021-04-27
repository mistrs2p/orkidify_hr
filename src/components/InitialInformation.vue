<template>
    <v-row>
        <div class="twoPart">
            <h2>اطلاعات اولیه</h2>
        </div>
    
        <div class="twoPart">
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
        </div>
    </v-row>
</template>

<script>
export default {
    props: ['gender', 'years', 'months']
}
</script>

<style>

</style>