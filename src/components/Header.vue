<template>
    <div id="header"> 
       <div class="logo">
          <a href="http://localhost:8080/#/home">Link every things</a>
       </div>
       <ul class="nav">
         <li class="selected">
           <a href="/">首页</a>
         </li>
         <li>
           <a href="/developer">开发者</a>
         </li>
         <li>
           <a href="/developer">探索</a>
         </li>
         <li>
           <a href="/developer">博客</a>
         </li>
         <li>
           <a href="/developer">联系我们</a>
         </li>
       </ul>
    </div>
</template>

<script>
export default {
  name: 'ms-header',
  data () {
    return {
      msg: '',
      name: '',
      id: 'testid',
      api: 'testapi'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#header {
    display: flex;
    position:fixed;
}
.logo {
    width:230px;
    justify-content:flex-start;
}
.nav {
    justify-content:flex-end;
    list-style-type:none;
    margin:0;
    padding:0;
    right:60px;
    top:10px;
    height:40px;
    line-height:40px;
}

</style>

