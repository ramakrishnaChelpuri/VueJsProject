<template>
    <navBar />
    <displayCars :cars="cars" />
    <webFooter />
</template>

<script>
    import navBar from './components/navBar.vue'
    import displayCars from './components/displayCars.vue'
    import webFooter from './components/webFooter.vue'


    export default {
        name: 'App',

        components: {
            navBar,
            displayCars,
            webFooter
        },

        data() {
            return {
                cars: []
            }
        },

        methods: {
            async fetchCars() {
                const response = await fetch("https://car-rental-service-website.herokuapp.com/api");
                const data = await response.json();
                console.log(data);
                return data.cars
            }
        },

        async created() {
            this.cars = await this.fetchCars()
        }
    }

</script>

<style>
    :root {
        font-family: 'Footlight MT';
        background-color: #14213d;
    }

    #app {
        font-family: 'Footlight MT';
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
    }
</style>