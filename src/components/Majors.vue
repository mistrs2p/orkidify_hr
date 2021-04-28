<template>
        <v-row>
            <div class="twoPart">
                <h2>مقطع تحصیلی (لطفا از آخرین مقطع تحصیلی شروع کنید)</h2>
            </div>
            <div class="twoPart">
                    <v-col
                        cols="6"
                    >
                    <v-text-field
                        :rules="[rules.required]"
                        label="رشته تحصیلی (اجباری)"
                    />
                </v-col>
                
                <v-col
                    cols="6"
                >
                    <v-select
                        :rules="[rules.required]"
                        label="مقطع تحصیلی (اجباری)"
                        :items="majors"
                    />
                </v-col>

                <v-col
                    cols="6"
                >
                    <v-text-field
                        :rules="[rules.required]"
                        label="نام دانشگاه (اجباری)"
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
            </div>
        </v-row>
</template>

<script>
export default {
 props: ['majors', 'years', 'rules']
}
</script>

<style>

</style>