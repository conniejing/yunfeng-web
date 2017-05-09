<template>
  <el-row>
    <el-col :span="24">
      <div class="grid-content bg-purple-dark clearfix">
        <div class="fl">
          <img class="logo" src="../common/images/logo.png" alt="logo" />
        </div>
        <div class="logo_title">云蜂</div>
        <ul class="fr">
          <li>Albee</li>
          <li>系统管理员</li>
          <li><a href="">退出</a></li>
        </ul>
      </div>
    </el-col>
  </el-row>
</template>
<style lang="scss" scoped>
  .el-row {
      color: #D7D7D7;
      .bg-purple-dark {
      background: #2C3D59;
    }
    .grid-content {
      border-radius: 0px;
      padding:0px 15px;
    }
    .logo {
    padding:3px 0;
    user-select:none;
    }
    .logo_title {
       user-select:none;
       float:left;
       height:36px;
       line-height:36px;
       margin:7px 13px;
     padding-left:15px;
     font-size:18px;
     letter-spacing:1px;
     font-weight:bold;
       border-left:1px solid #D7D7D7;
       vertical-align: middle;
    }
    li {
      float:left;
      height:50px;
      line-height:50px;
      padding:0 8px;
      font-size:14px;
      a {
        user-select:none;
        color:#D7D7D7;
      }
    }
  }
</style>
