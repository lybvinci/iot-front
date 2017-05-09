<template>
  <div id="deviceManager">
    <h1>{{ msg }}</h1>
    <h2>设备列表</h2>
    <div class="myDevice">
        <p>name:{{name}}</p>
        <p>id:{{id}}</p>
        <p>api:{{api}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      msg: '设备管理',
      name: 'test1',
      id: 'testid',
      api: 'testapi'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#deviceManager {
    position: relative;
    display: block;
    margin: auto;
    top: 64px;
    z-index: 1;
}
</style>

