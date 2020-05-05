<template>
  <div>
    <el-button type="infor" @click="logout">退出</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    logout () {
      window.sessionStorage.removeItem('token')
      this.$message.success('注销成功')
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped>
</style>
