<template>
  <v-app>
    <!--https://material.io/tools/icons/-->
    <v-toolbar color="teal lighten-2 white--text">
        <v-toolbar-side-icon 
          class="white--text"
          @click="exibe = !exibe"
        ></v-toolbar-side-icon>
        <v-toolbar-title>Barbearia</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-text-field
          placeholder="Pesquisar"
          append-icon="search"
          class="hidden-sm-and-down"
        ></v-text-field>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
          <v-btn to="/" flat class="white--text">Página Inicial</v-btn>
          <v-btn to="/perfil" flat class="white--text">Perfil</v-btn>
          <v-btn flat class="white--text">Link Three</v-btn>
        </v-toolbar-items>
    </v-toolbar>
    <v-navigation-drawer 
      absolute
      temporary
      v-model="exibe"
    >
      <v-toolbar color="teal lighten-2 white--text">
        <h1>Barbearia</h1>
      </v-toolbar>
      <v-divider></v-divider>
      <v-list dense>
        <v-list-tile to="/">
          <v-list-tile-action>
            <v-icon color="teal">dashboard</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            Início
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/login">
          <v-list-tile-action>
            <v-icon color="teal">person</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            Login
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/cartao">
          <v-list-tile-action>
            <v-icon color="teal">credit_card</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            Exemplo de Cartão
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
  
</template>
<script>
  export default {
    data(){
      return{
        exibe: false,
        logado: false
      }
    } 
  }
</script>

