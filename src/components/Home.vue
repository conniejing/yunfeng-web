<template>
  <div class="main-content">
    <v-header></v-header>
    <div class="main clearfix">
      <side-bar></side-bar>
      <div class="contentBox">
        <!-- 内容部分 -->
        <router-view></router-view>
      </div>
    </div>
  </div>
</template>
<script>
  import vHeader from '@/components/Header'
  import sideBar from '@/components/SideBar'
  export default {
    data () {
      return {

      }
    },
    components: {
      vHeader,
      sideBar
    }
  }
</script>
<style lang="scss" scoped>
  .main{
    width:100%;
    height:100%;
    .sidebar {
      width:200px;
      position: absolute;
      left:0;
      top:50px;
      height:calc(100% - 50px);
      background:#324157;
      overflow-y:auto;
    }
    .contentBox {
      box-sizing: border-box;
      width:100%;
      padding:15px 15px 15px 215px;
    }
  }
</style>
