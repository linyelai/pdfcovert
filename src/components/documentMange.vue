<template>
  <div class="document-manage">
       <div class="document-menu">
         <div class="document-name">   <el-input
        placeholder="文件名"
        v-model="documentName"
        clearable>
      </el-input>
         </div>
         <div class='search-document-btn'>
      <el-button type='primary' icon="el-icon-search">查询</el-button>
      </div>
       <div class='search-document-btn'>
      <el-button type='danger' icon="el-icon-delete">删除</el-button>
      </div>
       </div>
       <div class="dashborad-tab">
           <el-table
      :data="dataList"
      style="width: 100%">
      <el-table-column
      type="selection"
      width="55">
    </el-table-column>
      <el-table-column
        prop="id"
        label="ID"
        width="180">
      </el-table-column>
      <el-table-column
        prop="name"
        label="文件名"
        width="180">
      </el-table-column>
      <el-table-column
        prop="createTime"
        label="创建时间">
      </el-table-column>
      <el-table-column
        prop="updateTime"
        label="更新时间">
      </el-table-column>
    </el-table>
       </div>
       <div>
           <el-pagination
            background
            layout="prev, pager, next"
            :total="1000">
</el-pagination>
       </div>
  </div>
</template>
<script>
import Table from 'element-ui'
export default {
  name: 'DocumentManage',
  data() {
      return {
          dataList:[
              {
                  id:1,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
              {
                  id:2,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
              {
                  id:3,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              }
              ,{
                  id:4,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
              {
                  id:5,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
              {
                  id:6,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
              {
                  id:7,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
              {
                  id:8,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
               {
                  id:9,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              },
               {
                  id:10,
                  name:"test.pdf",
                  createTime:"2020-01-12",
                  updateTime:'2020-01-21'
              }
          ],
          documentName:''
      }
  },
  components: {}
}
</script>
<style>
 .document-name{
     width:200px;
     float: left;
 }
 .search-document-btn{
     width:100px;
     float: left;
 }
 .dashborad-tab{
     margin-top:10px;
 }
 .document-menu{
     height:40px;
 }
</style>
