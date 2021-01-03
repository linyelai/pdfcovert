<template>
  <div >
      <Top></Top>
  <div class="dashborad">
    <el-tabs value="documentManage">
    <el-tab-pane label="文档管理" name="documentManage">
        <DocumentManage></DocumentManage>
    </el-tab-pane>
    <el-tab-pane label="文件转换" name="filecovert" style="height:420px">
        <DataList></DataList>
    </el-tab-pane>
    <el-tab-pane label="个人中心" name="second">
        <PersonInfo></PersonInfo>
    </el-tab-pane>
  </el-tabs>
  </div>
    <Footer></Footer>

  </div>
</template>

<script>
import Top from './top'
import Footer from './footer'
import Nav from './nav'
import Tabs from 'element-ui'
import DocumentManage from './documentMange'
import PersonInfo from './person'
import DataList from './dataList'
export default {
  name: 'PersonCenter',
  data () {
    return {
     
    }
  },
  components:{
    Footer,
    Nav,
    Top,
    DocumentManage,
    PersonInfo,
    DataList
  }
}
</script>

<style>
.dashborad{
    width:100%;
    float: left;
    margin-left: 20px;
    margin-top: 10px;
    height:700px;
}
.nav-1{
    width:200px;
    float: left;
    margin-top: 10px;
}
</style>
