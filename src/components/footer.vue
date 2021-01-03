<template>
  <div class="footer">
      <copyRight></copyRight>
  </div>
</template>
<script>
import CopyRight from './copyRight'
export default {
  name: 'Footer',
  components: {CopyRight}
}
</script>
<style>
.footer{
    clear: both;
    height: 40px;
    margin-top: 20px;
    width:100%;

}
</style>
