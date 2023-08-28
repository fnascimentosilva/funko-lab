<template>
  <v-layout>
    <v-app-bar color="#d6249f">
      <v-app-bar-title> <router-link to="/" class="link title">Action Figures</router-link></v-app-bar-title>

      <v-btn icon>
        <router-link to="/carrinho" class="link">
        {{ this.$store.state.produtosCarrinho.length}}
          <v-icon color="#FFF">mdi-cart</v-icon>
        </router-link>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view></router-view>
    </v-main>
  </v-layout>
</template>

<style scoped>
.link{
  text-decoration: none;
}

.title{
  color: #fff;
  font-size: 30px;
}
</style>


