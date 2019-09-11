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
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>

    <v-footer
      color="indigo"
      dark
      app
    >
    <div style="width: 100%" v-if="$vuetify.breakpoint.smAndUp" class="d-flex justify-space-between">
      <span class="caption">LLPG Soluções ®</span>
      <span class="caption">Áreas Metropolitanas: 9999-9999  |  Demais localidades: 0800-999-9999</span>
      <span class="caption">&copy; 2019</span>
    </div>
    <div style="width: 100%" v-else class="d-flex justify-center">
      <span class="caption">LLPG Soluções ®</span>
    </div>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      fixed: true,
      title: 'LLPG - Controle de Frotas'
    }
  }
}
</script>
