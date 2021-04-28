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
                :rules="[rules.required]"
                label="جنسیت (اجباری)"
                :items="gender"
            />
            </v-col>
            <v-col
                cols="6"
            >
                <v-text-field
                    :rules="[rules.required]"
                    label="نام پدر (اجباری)"
                />
            </v-col>

            <v-col
                cols="6"
            >
                <v-text-field
                    :rules="[rules.required]"
                    label=" شماره شناسنامه (اجباری)"
                />
            </v-col>

            <v-col
                cols="6"
            >
            <v-text-field
                :rules="[rules.required]"
                label="کد ملی (اجباری)"
            />
            </v-col>

            <v-col
            cols="3"
            >
            <v-select 
                :rules="[rules.required]"
                label="سال تولد شناسنامه ای (اجباری)"
                :items="years"
            />
            </v-col>

            <v-col
            cols="6"
            >
            <v-select
                :rules="[rules.required]"
                label="ماه تولد (اجباری)"
                :items="months"
            />
            </v-col>

            <v-col
            cols="3"
            >
            <v-text-field
                :rules="[rules.required]"
                label="روز (اجباری))"
            />
            </v-col>

                    <v-col
            cols="3"
            >
            <v-select 
                :rules="[rules.required]"
                label="سال تولد حقیقی (اجباری)"
                :items="years"
            />
            </v-col>

            <v-col
            cols="6"
            >
            <v-select
                :rules="[rules.required]"
                label="ماه تولد (اجباری)"
                :items="months"
            />
            </v-col>

            <v-col
            cols="3"
            >
            <v-text-field
                :rules="[rules.required]"
                label="روز (اجباری))"
            />
            </v-col>
        </div>
    </v-row>
</template>

<script>
export default {
    props: ['gender', 'years', 'months', 'rules']
}
</script>

<style>

</style>