<template>
  <v-app>
    <v-content>
      <Layout/>
    </v-content>
  </v-app>
</template>

<script>
import Layout from './components/Layout'

export default {
  name: 'App',
  components: {
    Layout
  },
  data () {
    return {
      //
    }
  }
}
</script>

<style>
</style>