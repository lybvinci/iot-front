<template>
  <div>
    <div class="loginTitle">
    <h1>登录</h1> 
    <p> Connect the every things </p>
    </div>
    <form class="login" v-on:submit.prevent="submit">
      <div class="wrapContent">
        <div class="line">
            <div v-show="btn && !form.id">id不能为空</div>
            <input placeholder="输入你的用户名" size="30" v-model="form.id">
          </div>
          <div class="line">
            <div v-show="btn && !form.name">用户名不能为空</div>
            <input type="password" placeholder="输入你的密码" v-model="form.name">
        </div>
        <button>登录</button>
      </div>
      <div class="wrapContent">
        <p>简介。。。</p>
      </div>
    </form>
  </div>
</template>

<script>
import { mapActions } from 'vuex'
import { USER_SIGNIN } from '../store/user'
export default {
  name: 'login',
  data () {
    return {
      btn: false, // true 已经提交 false 没有提交
      form: {
        id: '',
        name: ''
      }
    }
  },
  methods: {
    ...mapActions([USER_SIGNIN]),
    submit () {
      this.btn = true
      if (!this.form.id || !this.form.name) {
        return
      }
      console.log(this.USER_SIGNIN)
      this.USER_SIGNIN(this.form)
      this.$router.replace({path: '/home'})
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
    font-size: 36px;
    padding-top: 30px;
    padding-left: 40px;
}
p {
    padding-left: 40px;
    font-size: 14px;
    ling-height: 30px;
}
.loginTitle {
    background-color: #E3F2FD;
    display: bolck;
    width: 100%;
    height: 160px;
    margin-top: 80px;
}
.login {
    padding: 50px;
    display: flex;
    text-align: center;
    background-color: #BBDEFB;
    box-shadow: 0px 5px 8px rgba(0,0,0,.3);
    .line {
        padding: 5px;
    }
}
button {
    padding: 0 20px;
    margin-top: 20px;
    line-height: 28px;
}
input {
    padding: 0 10px;
    line-height: 28px;
    outline: none;
    width: 210px;
    border: 0px;
    background-color: #BBDEFB;
    border-bottom: #009688 1px solid;
    margin: 10px;
}
.wrapContent {
    flex: 1;
}
</style>
