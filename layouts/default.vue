<template>
  <v-app dark>
    <v-navigation-drawer
      dark
      v-model="drawer"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      color="white"
      fixed
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-side-icon>
        <img src="/icons/car.png" height="40px" class="mx-5"/>
      </v-toolbar-side-icon>
      <v-toolbar-title v-text="title" class="body-1" />
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
      class="justify-space-between"
      color="indigo"
      dark
      app
    >
      <span class="caption">LLPG Soluções ®</span>
      <span class="caption">Áreas Metropolitanas: 9999-9999  |  Demais localidades: 0800-999-9999</span>
      <span class="caption">&copy; 2019</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: false,
      fixed: true,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      title: 'Controle de Frotas'
    }
  }
}
</script>
