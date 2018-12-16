<template>
    <v-container class="white">
        <h1 class="display-3 text-xs-center">How It Works?</h1>
        <v-layout row wrap class="py-5 featured">
            <v-flex sm7 class="mobileApp"></v-flex>
            <v-flex align-center sm5 class="py-4" fill-height>
                <v-list two-line align-center>
                    <v-list-tile class="pb-5 workingCards" avatar v-for="item in working" :key="item.icon">
                        <v-list-tile-avatar>
                            <v-icon class="teal lighten-2 white--text"> {{item.icon}} </v-icon>
                        </v-list-tile-avatar>
                        <v-list-tile-content>
                            <v-list-tile-title class="font-weight-medium text-uppercase">{{item.title}}</v-list-tile-title>
                            <v-list-tile-sub-title>{{item.content}}</v-list-tile-sub-title>
                        </v-list-tile-content>
                    </v-list-tile>
                </v-list>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>
export default {
    data(){
        return{
            working: [
                { icon: 'find_in_page', title: 'Find your Favourite Dish', content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime voluptatibus' },
                { icon: 'shopping_cart', title: 'Place your Order', content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime voluptatibus' },
                { icon: 'location_on', title: 'Tracing your order', content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime voluptatibus' },
            ]
        }
    }
}
</script>

<style scoped>

.mobileApp{
    background-image: url('/seamless.png');
    background-size: contain;
    background-position: center;
}
.workingCards{
    position: relative;
}

.workingCards::before{
    border-left: 1px solid #eee;
    position: absolute;
    top: 0;
    left: 35px;
    height: 100%;
    content: ""
}
.featured{
    min-height: 90vh;
}

</style>

