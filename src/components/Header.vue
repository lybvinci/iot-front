<template>
    <div id="header"> 
       <div class="logo">
          <a href="http://localhost:8080/#/home">Link every things</a>
       </div>
       <ul>
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
    left: 0px;    
    top: 5px;
    right: 0px;
    margin-left: 5px;
    margin-right: 5px;
    justify-content: space-around;
    align-content:space-between;
    width: auto;
    height: 62px;
    box-shadow: 0 1px 8px rgba(0,0,0,.3);
    z-index: 2;
    padding: 5px;
}
.logo {
    display: flex;
    align-items: center;
    margin-left: 10px;
    width: 150%;
    color: #2c3e50;
    font-weight: 500;
    font-size: 2em;
    font-family: "Microsoft YaHei", "Arial";
}
ul {
    display: flex;
    width: 50%;
    justify-content:space-around;
    margin-right: 5px;
    align-items: flex-end;
    list-style-type:none;
}

</style>

