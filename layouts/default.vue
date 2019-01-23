<template>
  <el-container class="container">
    <el-header 
      class="header" 
      height="197px">
      <my-header/>
    </el-header>
    <el-main>
      <nuxt/>
    </el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</template>

<script>
import myHeader from '../components/public/header/index'
export default {
  components: { myHeader }
}
</script>

<style scoped>
.container >>> .el-main {
  padding: 0;
  overflow: inherit;
}
.container {
  text-align: center;
}
.header {
  text-align: center;
  width: 100%;
  padding: 0;
}
</style>
