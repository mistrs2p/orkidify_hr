<template>
    <v-row>
        <div class="twoPart">
            <h2>نام شما</h2>
        </div>
        <div class="twoPart">
            <v-col
            cols="6"
            >
            <v-text-field
                :rules="[rules.required]"
                label="نام (اجباری)"
            />
            </v-col>

            <v-col
            cols="6"
            >
            <v-text-field
                :rules="[rules.required]"
                label="Name (اجباری)"
            />
            </v-col>
            <v-col
            cols="6"
            >
            <v-text-field
                :rules="[rules.required]"
                label="نام خانوادگی (اجباری)"
            />
            </v-col>

            <v-col
            cols="6"
            >
            <v-text-field
                :rules="[rules.required]"
                label="family (اجباری)"
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