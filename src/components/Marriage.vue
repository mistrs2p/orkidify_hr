<template>
        <v-row>
            <div class="twoPart">
                <h2>وضعیت تاهل</h2>
            </div>
            <div class="twoPart">
                <v-col
                    cols="6"
                >
                <v-select 
                    :rules="[rules.required]"
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
            </div>
        </v-row>
</template>

<script>
export default {
    props: ['marriage', 'majors', 'rules']
}
</script>

<style>

</style>