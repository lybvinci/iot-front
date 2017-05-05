<template>
  <div id="app">
    <ms-header></ms-header>
    <router-view></router-view>
  </div>
</template>
<script>
import MsHeader from '@/components/Header'
export default {
  name: 'app',
  components: {
    MsHeader
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
