<template>
  <div id="app">
    <ms-header></ms-header>
    <router-view></router-view>
    <ms-footer></ms-footer>
  </div>
</template>
<script>
import MsHeader from '@/components/Header'
import MsFooter from '@/components/Footer'
export default {
  name: 'app',
  components: {
    MsHeader,
    MsFooter
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
