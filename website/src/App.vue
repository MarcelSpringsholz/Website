<template>
  <v-app>
    <v-app-bar
      app
      dark
    >
      <v-btn large text to="/">MarcelS.</v-btn>
      <spacer/>
      <v-btn small text to="Video">Video</v-btn>
      <v-btn small text to="Photo">Photo</v-btn>
      <v-btn small text to="Projekt">Projekts</v-btn>

  
    </v-app-bar>

    <v-content>
      <Router-view/>
    </v-content>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {
  },

  data: () => ({
    //
  }),
};
</script>
