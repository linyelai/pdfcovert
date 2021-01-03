<template>
  <div class="person-info">
      <div class="account-line">
          <div class="account-label">账号</div><div class="account">test@gmail.com</div>
      </div>
      <div class="passwd-line">
          <div class="account-label">密码</div><div class="account">
              <el-input v-model='password' placeholder="密码" type="password" autocomplete="off" @input="updateView($event)">
                </el-input>
            </div> 
      </div>
  </div>
</template>
<script>
export default {
  name: 'PersonInfo',
  data() {
      return {
         password:'123456'

      }
  }
  }
</script>
<style>
.account-label{
    float: left;
    width:100px;
}
.account{
    float: left;
    margin-left: 40px;
    width:200px;
}
.person-info{
    margin-left: 200px;
    margin-top:100px;
}
.passwd-line{
    clear: both;
    margin-top:20px;
    height:48px;
}
.account-line{
    height:48px;
}
</style>
