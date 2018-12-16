<template>
  <div class="dashboard">
        <v-layout align-center justify-center row wrap class="dash" >
            <v-flex sm6 class="pa-5 " >
                <h1 class="display-3">Experience a world of food</h1>
                <p class="headline mt-2">Anywhere - Anytime</p>
                <v-btn round large >Get Started</v-btn>
            </v-flex>
            <v-flex sm6 class="dashImg" >
            </v-flex>
        </v-layout>
        <whyUs />
        <featuredCont />
  </div>
</template>

<script>
import whyUs from '@/components/whyUs'
import featuredCont from '@/components/featuredCont'
export default {
    components: {
        whyUs,
        featuredCont
    }
  
}
</script>

<style scoped>
    .dash{
        /* background-color: crimson; */
    }
    .dashImg{
        min-height: 70vh;
        background: url('http://en.zopix.net/image_upload/201932-dish-restaurant-dining-food.jpg');
        background-size: cover;
        background-position: right;
        transform: skewX(200px)
    }
</style>
