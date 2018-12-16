<template>
    <v-layout row align-center class="commentsSection pa-5">
        <v-flex xs6 offset-xs5>
            <v-card flat color="white" class="grey--text">
              <v-layout>
                <v-flex xs3 class="pa-3">
                  <v-img
                    src="https://cdn.vuetifyjs.com/images/cards/foster.jpg"
                    height="125px"
                    contain
                  ></v-img>
                </v-flex>
                <v-flex xs9>
                  <v-card-title primary-title>
                    <div>
                      <div class="headline">Oreki Houtarou</div>
                      <div>Tokyo, Japan</div>
                    </div>
                  </v-card-title>
                </v-flex>
              </v-layout>
              <v-layout class="px-3">
                  <v-flex xs12>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit eveniet laboriosam corporis, ex quia odio impedit tempore facilis</p>
                </v-flex>
              </v-layout>
              <v-card-actions class="px-3 pb-3 yellow--text">
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
                <v-icon>star_border</v-icon>
              </v-card-actions>
            </v-card>
          </v-flex>

    </v-layout>
</template>

<style scoped>
.commentsSection{
    height: 70vh;
    background: url('/comments.png');
    background-position: center;
    background-size: cover;
}
</style>
