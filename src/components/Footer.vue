<template>
    <div id="footer"> 
       <div class="logo">
          <a href="http://localhost:8080/#/home">Link every things</a>
       </div>
    </div>
</template>

<script>
export default {
  name: 'ms-footer',
  data () {
    return {
      msg: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#footer {
    display: flex;
    background-color: #0d47a1;
    justify-content: center;
    width: auto;
    align-items: center;
    height: 140px;
    margin-top: 50px;
    padding: 5px;
    box-shadow: 0px 5px 8px;
}
a {
    color: #a0a0a0;
    font-weight: 500;
    font-size: 2em;
}
</style>

