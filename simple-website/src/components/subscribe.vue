<template>
    <v-layout align-center justify-center class="teal lighten-2 pa-5 white--text subscribe">
        <v-flex xs5 class="text-xs-center">
            <h1>Don't miss out on the latest</h1>
            <v-text-field dark class="white--text" placeholder="enter your email address" append-icon="arrow_forward">
            </v-text-field>
        </v-flex>
    </v-layout>
</template>

<script>
export default {
    
}
</script>

<style scoped >
.subscribe{
    height: 40vh;
}
.subscribe.primary--text{
    color: crimson !important;
    caret-color: crimson;
}

</style>
