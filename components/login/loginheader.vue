<template>
  <div class="header">
    <el-row :gutter="0">
      <el-col :span="24">
        <div class="grid-content bg-purple">
          <img src="http://s0.meituan.net/bs/file/?f=fe-sso-fs:build/assets/sp-retina.b95a7dd.png">
        </div>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {}
</script>

<style scoped>
.header {
  width: 1000px;
  margin: 0 auto;
  height: 50px;
  padding: 40px 40px 20px;
}
.header img {
  width: 80px;
  height: 55px;
}
</style>
