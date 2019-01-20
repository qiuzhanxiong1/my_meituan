<template>
  <el-row 
    :gutter="0" 
    class="topbar">
    <el-col :span="4"><header-geo/></el-col>
    <el-col :span="3"><header-user/></el-col>
    <el-col :span="17"><header-nav/></el-col>
  </el-row>
</template>
<script>
import HeaderGeo from './geo'
import HeaderUser from './user'
import HeaderNav from './nav'
export default {
  components: {
    HeaderGeo,
    HeaderUser,
    HeaderNav
  }
}
</script>
<style scoped>
.topbar {
  width: 1200px;
  margin: 0 auto;
  color: #666;
}
</style>
