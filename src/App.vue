<template>
  <v-app>
    <v-app-bar app color="info" dark>
      <v-toolbar-title>Edutecno DashBoard</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text to="/home" width="90px" class="mr-2">Home</v-btn>
      <v-btn text to="/">Login</v-btn>
    </v-app-bar>
    <v-main>
      <router-view></router-view>
    </v-main>
    <v-card height="150">
      <v-footer absolute class="font-weight-medium" color="info">
        <v-col class="text-center" cols="12">
          {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
        </v-col>
      </v-footer>
    </v-card>
  </v-app>
</template>

<script>

export default {
  name: 'App',
};
</script>
