<template>
  <v-app light>
      <v-toolbar dark class="primary">
          <v-toolbar-side-icon></v-toolbar-side-icon>
          <v-toolbar-title light>Vue Analytics</v-toolbar-title>
          <v-spacer></v-spacer>
          <v-text-field
                  label="Insérer votre Oauth Google client ID..."
                  single-line
                  append-icon="search"
                  dark
                  hide-details
          ></v-text-field>
      </v-toolbar>
      <v-container>
          <router-view></router-view>
      </v-container>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        clipped: false,
        drawer: true,
        fixed: false,
        items: [
          { icon: 'bubble_chart', title: 'Inspire' }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: 'Vuetify.js'
      }
    }
  }
</script>

<style lang="stylus">
  @import './stylus/main'
</style>
