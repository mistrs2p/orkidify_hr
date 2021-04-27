<template>
    <v-row>
        <div class="twoPart">
            <h2>طرح و سربازی</h2>
        </div>

        <div class="twoPart">
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
        </div>
    </v-row>
</template>

<script>
export default {
    props: ['military']
}
</script>

<style>

</style>