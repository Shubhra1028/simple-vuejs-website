<template>
    <v-toolbar flat class="white">
      <v-toolbar-title class="headline text-uppercase orange--text">
        <span>F</span>
        <span class="font-weight-light">oozi</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn class="hidden-xs-and-down" flat v-for="item in navItems" :key="item" >
        <span class="mr-2"> {{item}} </span>
      </v-btn>
      <v-btn flat target="_blank" >
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-toolbar>
</template>

<script>
export default {
    data(){
        return {
            drawer: false,
            navItems : [ 'Explore Food', 'Help', 'Blog' ]
        }
    }
}
</script>

