<template>
  <v-app>
    <navBar/>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import navBar from './components/NavBar'

export default {
  name: 'App',
  components: {
    navBar
  },
  data () {
    return {
      //
    }
  },
  mounted () {
    this.$vuetify.theme.primary = '#4caf50'
  }
}
</script>
