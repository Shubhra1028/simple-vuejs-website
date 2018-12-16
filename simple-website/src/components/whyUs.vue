<template>
    <v-container>
        <div class="my-5 text-xs-center">
            <h2 class="display-3">Why Order with Foozi</h2>
            <p class="headline" xs12>Making your life easier is our top priority</p>
        </div>
        <v-layout row wrap>
            <v-flex xs12 sm4 lg4 v-for="(item, id) in cardDetails" :key="id">
                <v-card justify-center class="text-xs-center ma-3" height="300px">
                    <v-responsive class="pt-4">
                        <v-avatar size="100" class="grey lighten-2">
                        <img :src="item.avatar" alt="">
                        </v-avatar>
                    </v-responsive>
                    <v-card-title>
                        <h3 class="text-xs-center"> {{item.title}} </h3>
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
                { avatar: '', title: 'Fast Delivery & Safe Delivery', content: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse iure ea, cupiditate amet voluptates' },
                { avatar: '', title: 'Cheaper and better with Group Orders', content: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse iure ea, cupiditate amet voluptates' },
                { avatar: '', title: 'Order from Great Restaurants near You', content: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Esse iure ea, cupiditate amet voluptates' },
            ]
        }
    }
}
</script>
