<template>
  <v-app app>
    <!--<v-app-bar app>
      <v-toolbar-title class="headline text-uppercase">
        <span>Vuetify</span>
        <span class="font-weight-light">MATERIAL DESIGN</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        text
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
      >
        <span class="mr-2">Latest Release</span>
      </v-btn>
    </v-app-bar>-->
    <navbar></navbar>
    <v-content>
     <router-view></router-view> 
    </v-content>
    
  </v-app>
</template>

<script>
import navbar from './components/navbar'

export default {
  name: 'App',
  components: {
    navbar
  },
  data: () => ({
    //
  }),
};
</script>
