<template>
  <div class="profile">
     <div class="sign-up">
       <span><a href="/signup">注册</a> </span>
    </div>
  <div class="sign-in"><a href="/login">登录 </a></div>
  </div>
</template>
<script>
export default {
  name: 'Profile'
}
</script>

<style>
.profile{
    height: 40px;
    width:120px;
    float:right;

}
.sign-up{

    margin-right: 4px;
    vertical-align: middle;
    float: left;
    font-size: 12px;
    height: 40px;
    margin-top: 10px;
}
.sign-in{
    margin-right: 4px;
    float: left;
    font-size: 12px;
    margin-top: 10px;
}
.profile a{
    text-decoration: none;
    color:#000000;
}
</style>
