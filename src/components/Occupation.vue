<template>
    <v-row>
        <div class="twoPart">
            <h2>سوابق شغلی</h2>
        </div>
        <div class="twoPart">
            <v-col
            cols="6"
            >
            <v-text-field 
                :rules="[rules.required]"
                label="عنوان شغلی (اجباری)"
            />
            </v-col>
            
            <v-col
            cols="6"
            >
            <v-text-field 
                :rules="[rules.required]"
                label="نام شرکت (اجباری)"
            />
            </v-col>
            <v-col
            cols="3"
            >
            <v-select 
                :rules="[rules.required]"
                label="ماه ورود (اجباری)"
                :items="months"
            />
            </v-col>
            <v-col
            cols="3"
            >
            <v-select 
                :rules="[rules.required]"
                label="سال ورود (اجباری)"
                :items="years"
            />
            </v-col>
            <v-col
            cols="3"
            >
            <v-select 
                :rules="[rules.required]"
                label="ماه خروج (اجباری)"
                :items="months"
            />
            </v-col>
            <v-col
            cols="3"
            >
            <v-select 
                :rules="[rules.required]"
                label="سال خروج (اجباری)"
                :items="years"
            />
            </v-col>
            <v-col
            cols="12"
            >
            <v-text-field 
                :rules="[rules.required]"
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
        </div>
    </v-row>
</template>

<script>
export default {
    props: ['years', 'months', 'rules']
}
</script>

<style>

</style>