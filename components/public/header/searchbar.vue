<template>
  <div class="header-search">
    <el-row 
      :gutter="0" 
      class="search-content">
      <el-col :span="4">
        <div class="icon">
          <img src="http://s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/logo.png">
        </div>
      </el-col>
      <el-col :span="20">
        <search/>
      </el-col>
    </el-row>
  </div>
</template>
<script>
import Search from './search'
export default {
  components: {
    Search
  }
}
</script>
<style scoped>
.header-search {
  width: 100%;
  background-color: #fff;
}
.search-content {
  width: 1200px;
  margin: 0 auto;
}
.icon {
  width: 126px;
  height: 46px;
  margin-top: 30px;
}
.icon img {
  width: 100%;
  height: 100%;
}
</style>
