<template>
  <v-app>
    <!--https://material.io/tools/icons/-->
    <v-toolbar color="teal lighten-2 white--text">
        <v-toolbar-side-icon class="white--text"></v-toolbar-side-icon>
        <v-toolbar-title>Barbearia</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-text-field
          placeholder="Pesquisar"
          append-icon="search"
          class="hidden-sm-and-down"
        ></v-text-field>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
          <v-btn flat class="white--text">Link One</v-btn>
          <v-btn flat class="white--text">Link Two</v-btn>
          <v-btn flat class="white--text">Link Three</v-btn>
        </v-toolbar-items>
    </v-toolbar>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>
