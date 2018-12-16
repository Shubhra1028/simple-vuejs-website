<template>
    <v-container class="my-5">
        <div class="my-5 text-xs-center">
            <h2 class="display-3">Why Order with Foozi</h2>
            <p class="headline" xs12>Making your life easier is our top priority</p>
        </div>
        <v-layout row wrap>
            <v-flex xs12 sm4 lg4 v-for="(item, id) in cardDetails" :key="id">
                <v-card justify-center class="text-xs-center ma-3" min-height="300px">
                    <v-responsive class="pt-4">
                        <v-avatar size="200" class="grey lighten-2">
                        <img :src="item.avatar" alt="">
                        </v-avatar>
                    </v-responsive>
                    <v-card-title  class="text-xs-center">
                        <h3 class="text-xs-center fullWidth"> {{item.title}} </h3>
                        <p> {{item.content}} </p>
                    </v-card-title>
                </v-card>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    data(){
        return{
            cardDetails: [
                { avatar: 'https://image.freepik.com/free-vector/pizza-delivery-on-scooter_23-2147674077.jpg', title: 'Fast Delivery & Safe Delivery', content: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse iure ea, cupiditate amet voluptates' },
                { avatar: 'https://media.licdn.com/media-proxy/ext?w=800&h=800&hash=5cPt%2F9NXEh7RAx9OUuU1pkdUQr4%3D&ora=1%2CaFBCTXdkRmpGL2lvQUFBPQ%2CxAVta5g-0R6nlh8Tw1It6a2FowGz60oISIfYC2G8G2f1spyfNT-tdoDSfLqhpktOdS8BkgIkKeL2VmiwUcuxPoiZG4Uv_ZKwI-acb1EJXTcu3XAbqYMZHwA3t7K8Xa6jRGhBwO0FPGrvELjPRXELMiE8z-GZCquKJUsg7HCufemkS-9df4F28dRdjg5n8cHNMv8X0r5HwT1C7G6u95qjJ2g23qOkDWabNGlhKGv0Ye4Tv6m3-jCYugnWsWOE9NfIEoiKPIwe_Q', title: 'Cheaper and better with Group Orders', content: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse iure ea, cupiditate amet voluptates' },
                { avatar: 'https://us.123rf.com/450wm/yupiramos/yupiramos1511/yupiramos151102263/47595674-stock-vector-food-delivery-design-vector-illustration-eps10-graphic.jpg?ver=6', title: 'Order from Great Restaurants near You', content: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse iure ea, cupiditate amet voluptates' },
            ]
        }
    }
}
</script>


<style scoped>
.fullWidth{
    width: 100%;
}
</style>
