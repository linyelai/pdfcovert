<template>
  <div >
    <Top></Top>
    <div class="sign-in-container">
      <div class="sign-container-logo">

      </div>
    <div class="sign-in-form">
      <div class="form-head">

      </div>
      <div class="sign-in-username-input">
      <el-input
        placeholder="账号"
        v-model="username"
        clearable>
      </el-input>
      </div>
       <div class="sign-in-passwd-input">
      <el-input
        placeholder="密码"
        v-model="passwd"
        type='password'
        clearable>
      </el-input>
      </div>
      <div class="remember-me-container">
        <div class="remember-me">
             <el-radio v-model="rememberMe" label="1">记住我</el-radio>
        </div>
          <div class="forget-pass">
            <a href="#">忘记密码</a>
          </div>
      </div>
      <div class="sign-in-button">
      <el-button type='primary' v-on:click="signIn">登录</el-button>
      </div>
      <div class="sign-up-tips">
      <span>还没有账号？<a href="#">现在注册</a></span>
      </div>
    </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import Top from './top'
import Footer from './footer'
import Input from 'element-ui'
import Button from 'element-ui'
import Radio from 'element-ui'
export default {
  name: 'Login',
  data () {
    return {
      username: '',
      passwd: '',
      rememberMe:false,
    }
  },
  components:{
    Top,
    Footer
  },
  methods:{
    signIn(){
      console.log("sign in")
      this.$router.replace('/personCenter')
    }
  }
}
</script>

<style>
.sign-container-logo{
  float: left;
  width:60%;
  height:640px;
}
  .sign-in-form{
    width:400px;
    height:640px;
    box-shadow: 2px 2px 10px #909090;
    background-color: #ffffff;
    float: left;
  }
  .sign-in-container{
    margin-top:10px;
    height:650px;
  }
  .form-head{
    height:40px;
  }
  .sign-in-username-input{
    width:300px;
    margin-top:150px;
    margin-left: 50px;
  }
  .sign-in-passwd-input{
    width: 300px;
    margin-top: 20px;
    margin-left: 50px;
  }
  .sign-in-button{
    width:300px;
    margin-left: 50px;
    margin-top: 20px;
  }
  .sign-in-button button{
    width:300px;
  }
  .remember-me{
    float: left;
    margin-left: 50px;
  }
  .forget-pass{
    float: left;
    margin-left: 100px;
  }
  .forget-pass a{
    text-decoration: none;
    color:#838383;
  }
  .remember-me-container{
    height: 40px;
    margin-top: 20px;
  }
  .sign-up-tips{
    height:40px;
    margin-top: 20px;
  }
</style>
