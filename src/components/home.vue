<template>
  <div>
    <el-button @click="logout">退出</el-button>
  </div>
</template>

<script>
  export default {
    name: 'home',
    methods:{
      logout(){
        window.sessionStorage.removeItem('token')
        this.$router.push('/login')
      }
    }
  }
</script>

<style scoped>

</style>
