<template>
  <div>
    {{msg}}
    <button>
      <router-link to="/">点击我跳转</router-link>
    </button>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        msg: '我是登录页面'
      }
    },
    methods: {
    }
  }
</script>
