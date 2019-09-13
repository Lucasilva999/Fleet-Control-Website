<template>
  <v-app dark>
    <v-app-bar
      color="white"
      fixed
      app
    >
      <img src="/icons/car.png" height="40px" class="mx-5"/>
      <v-toolbar-title v-text="title" class="body-1" v-if="$vuetify.breakpoint.smAndUp" />
      <v-spacer />
      <v-btn color="black" text>
        <v-icon left>perm_identity</v-icon>
        Registrar 
      </v-btn>
      <v-btn color="black" text>
        Entrar
        <v-icon>chevron_right</v-icon>
      </v-btn>
    </v-app-bar>

    <Carousel/>

    <v-content style="padding: 32px;">
      <v-container>
        <nuxt/>
      </v-container>
    </v-content>

    <Footer/>
  </v-app>
</template>

<script>
import Carousel from '../components/LayoutItems/Carousel';
import Footer from '../components/LayoutItems/Footer';

export default {
  components: { Carousel, Footer },
  data () {
    return {
      fixed: true,
      title: 'LLPG - Controle de Frotas'
    }
  }
}
</script>
