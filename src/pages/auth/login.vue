<template>
  <div @keyup.enter="login()" style="margin-top:150px;">
    <el-row :gutter="20">
      <el-col :span="6" :offset="9">
          <el-form :model="loginInfo" ref="loginInfo" label-width="100px">
          <el-form-item label="用户名">
            <el-input type="text" v-model.trim="loginInfo.username" auto-complete="off"></el-input>
          </el-form-item>
          <el-form-item label="密码">
            <el-input type="password"  v-model.trim="loginInfo.password" auto-complete="new-password"></el-input>
          </el-form-item>
          <el-form-item class="text-center">
            <el-button type="primary" @click="login()">登录</el-button>
          </el-form-item>
        </el-form>
      </el-col>
    </el-row>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        loginInfo: {
          username: '',
          password: ''
        }
      }
    },
    methods: {
      login () {
        this.$router.push('/')
      }
    }
  }
</script>
