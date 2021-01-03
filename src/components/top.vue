<template>
  <div class="top">
      <div class="go-home">
          <a href="/home">首页</a>
      </div>
      <Profile></Profile>
  </div>
</template>
<script>
import Profile from './profile.vue'
export default {
  name: 'Top',
  components: {Profile}
}
</script>

<style>
.top{
    height: 40px;
    border-bottom: 1px solid rgba(211, 209, 209, 0.6);
}
.go-home{
    width:40px;
    float: left;
    margin-top: 10px;
    margin-left: 60px;
}
.go-home a{
    font-size: 14px;
    text-decoration: none;
}
</style>
