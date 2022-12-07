<template>
    <v-container class="displayCars">
        <v-row>
        <v-col v-for="car in cars" :key="car.id">
            <carDetails :car="car" />
        </v-col>
        </v-row>
  </v-container>
</template>


<script>
import carDetails from './carDetails.vue'

export default {
    name: 'displayCars',
    components : {
        carDetails
    },
    props:{
        cars: Array
    }
}
</script>


<style>
    .displayCars {
        display: grid;
        background-color: #5fa9f7;
        padding: 10px;
        margin: 10px;
    }
</style>
