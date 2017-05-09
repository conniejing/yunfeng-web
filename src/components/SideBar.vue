<template>
  <div class="sidebar">
    <el-menu mode="vertical" default-active="1" class="el-menu-vertical-demo" theme="dark">
      <el-menu-item :index="item.indexed" v-for="(item,index) in menus" :key="index">
        <router-link :to="item.link">{{item.name}}</router-link>
      </el-menu-item>
    </el-menu>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        menus: [
          {
            name: '看板',
            indexed: '1',
            link: '/'
          },
          {
            name: '事件',
            indexed: '2',
            link: '/'
          },
          {
            name: '用户',
            indexed: '3',
            link: '/'
          },
          {
            name: '留存',
            indexed: '4',
            link: '/'
          }
        ]
      }
    },
    methods: {
      handleOpen (key, keyPath) {
        console.log(key, keyPath)
      },
      handleClose (key, keyPath) {
        console.log(key, keyPath)
      }
    }
  }
</script>
<style lang="scss" scoped>
  .sidebar{
    .el-menu{
      border-radius:0;
      .el-submenu .el-menu-item{
        padding:0;
      }
      li.el-menu-item a{
        display:block;
        position:relative;
      }
      li.el-menu-item.is-active {
        a{
          color:#fff;
        }
      }
    }
  }
</style>
