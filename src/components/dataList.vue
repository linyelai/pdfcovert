<template>
  <div class="data-list">
     <div class="data-item" v-bind:key="item" v-for="item in dataList" >
        {{item.name}}
     </div>
  </div>
</template>
<script>
export default {
  name: 'DataList',
  data() {
      return {
          dataList:[
              {
                  name:"pdf编辑"
              },
              {
                  name:"pdf转换图片"
              },
              {
                  name:"word转换pdf"
              },
              {
                  name:"图片转换pdf"
              }
          ]
      }
  },
}
</script>

<style>
.data-list{
    display: flex;
    width:90%;
    margin:0 auto;

}
.data-item{
    width:400px;
    height: 400px;
    background-color: #ffffff;
    margin-left: 12px;
    box-shadow: 2px 2px 10px #909090;

}
</style>
