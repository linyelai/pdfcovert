<template>
  <div >
<Top></Top>
<Overview></Overview>
<DataList></DataList>
<Footer></Footer>
  </div>
</template>

<script>
import Top from './top'
import Footer from './footer'
import Overview from './overview'
import DataList from './dataList'
export default {
  name: 'Home',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    Top,
    Footer,
    Overview,
    DataList
  }
}
</script>

<style>
 *{
   margin:0 0 0 0 ;
 }
</style>
