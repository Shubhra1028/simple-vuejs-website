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
        <WhyUs />
        <FeaturedCont />
        <HowItWorks />
        <Comments />
        <Subscribe />
        <Footer />
  </div>
</template>

<script>
import WhyUs from '@/components/whyUs'
import FeaturedCont from '@/components/featuredCont'
import HowItWorks from '@/components/howItWorks'
import Comments from '@/components/comments'
import Subscribe from '@/components/subscribe'
import Footer from '@/components/footer'

export default {
    components: {
        WhyUs,
        FeaturedCont,
        HowItWorks,
        Comments,
        Subscribe,
        Footer
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
