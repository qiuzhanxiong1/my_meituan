<template>
  <div class="header-index">
    <el-row 
      :gutter="0"
      class = "top-header"
    >
      <el-col>
        <top-bar/>
      </el-col>
    </el-row>
    <el-row 
      :gutter="0"
      class = "search-header"
    >
      <el-col>
        <search-bar/>
      </el-col>
    </el-row>
  </div>
</template>
<script>
import topBar from './topbar'
import searchBar from './searchbar'
export default {
  components: {
    topBar,
    searchBar
  }
}
</script>
<style scoped>
.header-index {
  width: 100%;
}
.top-header {
  width: 100%;
  height: 40px;
  line-height: 40px;
  background-color: #f8f8f8;
  text-align: center;
}
</style>
