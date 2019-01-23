<template>
  <div class="index">
    <el-row 
      :gutter="0" 
      class="index-row">
      <el-col :span="5">
        <menu-nav/>
      </el-col>
      <el-col :span="19">
        <menu-list/>
      </el-col>
    </el-row>
    <el-row :gutter="0">
      <el-col :span="24">
        <menu-detail/>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import menuNav from '../components/index/menunav'
import menuList from '../components/index/menulist'
import menuDetail from '../components/index/menudetail'
export default {
  components: {
    menuNav,
    menuList,
    menuDetail
  }
}
</script>

<style scoped>
.index {
  width: 100%;
  background-color: #f8f8f8;
  padding: 0px;
}
.index-row {
  width: 1200px;
  margin: 0 auto;
}
</style>
