<template>
  <div class="dashboard white">
        <v-layout align-center justify-center row wrap class="dash" >
            <v-flex sm6 class="pa-5 " >
                <h1 class="display-3 white--text">Experience a world of food</h1>
                <p class="headline mt-2 white--text">Anywhere - Anytime</p>
                <v-btn round large >Get Started</v-btn>
            </v-flex>
            <v-flex sm6 class="dashImg" >
            </v-flex>
        </v-layout>
        <whyUs />
        <featuredCont />
        <howItWorks />
        <comments />
  </div>
</template>

<script>
import whyUs from '@/components/whyUs'
import featuredCont from '@/components/featuredCont'
import howItWorks from '@/components/howItWorks'
import comments from '@/components/comments'

export default {
    components: {
        whyUs,
        featuredCont,
        howItWorks,
        comments
    }
  
}
</script>

<style scoped>
    .dash{
        background: url('/dash.png');
        background-size: cover;
        background-position: center
    }
    .dashImg{
        min-height: 70vh;
        background-size: cover;
        background-position: right;
        transform: skewX(200px)
    }
</style>
