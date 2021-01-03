<template>
  <div class="left-nav">

<el-menu class="el-menu-vertical">
      <el-submenu index="1">
        <template slot="title">
          <i class="el-icon-location"></i>
          <span>文件管理</span>
        </template>
      </el-submenu>
      <el-menu-item index="2">
        <i class="el-icon-menu"></i>
        <span slot="title">个人中心</span>
      </el-menu-item>
    </el-menu>

  </div>
</template>

<script>
import NavMenu from 'element-ui'
export default {
  name: 'Nav',
  data () {
    return {
     
    }
  }
}
</script>

<style>
.left-nav{
    width:200px;
    height:400px;
    float: left;
}
</style>
