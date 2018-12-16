<template>
    <div>
        <v-layout class="featuredCont white" >
            <v-flex md6 class="pa-5 mt-5" >
                <v-container >
                    <h1 md4 class="display-2">Featured Items on Month</h1>
                    <p md6 class="subheading mt-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis quidem laborum laboriosam, est natus impedit quia ratione incidunt.</p>
                    <v-btn large class="mt-4">
                        <p class="caption">Available on <br /><span class="title">App Store</span> </p>
                    </v-btn>
                    <v-btn large class="mt-4">
                        <p class="caption">Available on <br /><span class="title">App Store</span> </p>
                    </v-btn>
                </v-container>
            </v-flex>
            <v-flex class="featuredImgGrid" >
                    <v-flex v-for="(item, id) in featuredCards" :key="id">
                        <v-card >
                            <v-img :src="item.src" :alt="item.title" height="150px" />
                            <v-card-actions>
                                <h3> {{item.title}} </h3>
                                <v-spacer></v-spacer>
                                <v-btn icon>
                                    <v-icon class="pink--text">favorite</v-icon>
                                </v-btn>
                            </v-card-actions>
                        </v-card>
                    </v-flex>
            </v-flex>
        </v-layout>
    </div>
</template>

<script>
export default {
    data(){
        return{
            featuredCards: [
                {src: 'https://keyassets-p2.timeincuk.net/wp/prod/wp-content/uploads/sites/50/2017/01/Prawn-Cocktail.jpg', title: 'Prawn Cocktail', price: '120' },
                {src: 'https://cdn-image.myrecipes.com/sites/default/files/styles/4_3_horizontal_-_1200x900/public/strawberry-bruschetta-sl.jpg?itok=NN73olQh', title: 'Strawberry Bruschetta', price: '110' },
                {src: 'http://howmanycaloriescounter.com/wp-content/uploads/2015/08/blue-cheese-puffs.jpg', title: 'Yummy Finger Food', price: '180' },
                {src: 'http://blog.byoh.in/wp-content/uploads/2016/04/Starter2.jpeg', title: 'Papdi chaat', price: '99' },
                {src: 'http://beta.lekhafoods.com/media/1272707/france-starters-fried-camembert.jpg', title: 'Fried Camembert', price: '200' },
                {src: 'https://blog.udemy.com/wp-content/uploads/2014/06/bigstock-Croissants-51957457.jpg', title: 'Dummy Food', price: '210' },
                {src: 'https://static-communitytable.parade.com/wp-content/uploads/2016/02/Corn-Dog-Mini-Muffins1.jpg', title: 'Pie love', price: '190' },
            ]
        }
    }
}
</script>


<style scoped>
.featuredCont{
    height: 100vh;
    background-image: url('/featured.png');
    background-color: #fff;
    background-size: 100% 98%;
    background-position: bottom;
    margin: 1in 0;
}

.featuredImgGrid{
    width: 80vw;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-column-gap: 10px;
    grid-template-areas: 
    ". two ."
    ". two thr"
    "one two thr"
    "one . thr"
    "one fyv ."
    ". fyv six"
    "fou fyv six"
    "fou . six"
    "fou sev ."
    ". sev .";
}

.featuredImgGrid>div>div{
    height: 100%;
}

.featuredImgGrid>div:nth-child(1){grid-area: one}
.featuredImgGrid>div:nth-child(2){grid-area: two}
.featuredImgGrid>div:nth-child(3){grid-area: thr}
.featuredImgGrid>div:nth-child(4){grid-area: fou}
.featuredImgGrid>div:nth-child(5){grid-area: fyv}
.featuredImgGrid>div:nth-child(6){grid-area: six}
.featuredImgGrid>div:nth-child(7){grid-area: sev}


</style>

