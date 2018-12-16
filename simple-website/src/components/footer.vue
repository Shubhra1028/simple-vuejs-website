<template>
  <v-footer height="auto" >
    <v-card class="flex" flat tile>
      <v-card-title class="white py-5">
        <v-flex sm9 class="display-2 text-uppercase orange--text">
        <span>F</span>
        <span class="font-weight-light">oozi</span>
        </v-flex>
        <v-spacer></v-spacer>

        <v-flex v-for="icon in icons" :key="icon" class="mx-3"  >
          <v-icon size="24px">{{ icon }}</v-icon>
        </v-flex>
      </v-card-title>

      <v-card-actions class="white justify-center">
        <v-btn flat v-for="item in navItems" :key="item" >
            <span class=""> {{item}} </span>
        </v-btn>
          <v-spacer />
        &copy;2018 — <strong>Vuetify</strong>
      </v-card-actions>
    </v-card>
  </v-footer>
</template>

<script>
export default {
    data(){
        return{
            icons: [ 'duo', 'android', 'chat'  ],
            navItems : [ 'Explore Food', 'Help', 'Blog' ]
        }
    }
}
</script>
