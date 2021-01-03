<template>
  <div >
    <Top></Top>
    <div class="sign-up-container">
      <div class="sign-container-logo">

      </div>
    <div class="sign-up-form">
      <div class="form-head">
      </div>
      <div class="sign-up-username-input">
      <el-input
        placeholder="账号"
        v-model="username"
        clearable>
      </el-input>
      </div>
       <div class="sign-up-passwd-input">
      <el-input
        placeholder="密码"
        v-model="passwd"
        clearable>
      </el-input>
      </div>
      <div class="sign-up-button">
      <el-button type='primary'>注册</el-button>
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
  }
}
</script>

<style>
.sign-container-logo{
  float: left;
  width:60%;
  height:640px;
}
  .sign-up-form{
    width:400px;
    height:500px;
    box-shadow: 2px 2px 10px #909090;
    background-color: #ffffff;
    float: left;
  }
  .sign-up-container{
    margin-top:10px;
    height:550px;
  }
  .form-head{
    height:40px;
  }
  .sign-up-username-input{
    width:300px;
    margin-top:150px;
    margin-left: 50px;
  }
  .sign-up-passwd-input{
    width: 300px;
    margin-top: 20px;
    margin-left: 50px;
  }
  .sign-up-button{
    width:300px;
    margin-left: 50px;
    margin-top: 20px;
  }
  .sign-up-button button{
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
