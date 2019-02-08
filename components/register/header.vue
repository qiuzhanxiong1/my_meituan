<template>
  <div class="header">
    <el-row
      :gutter="0"
      class="header-info">
      <el-col :span="6">
        <div class="grid-content bg-purple">
          <img src="http://s0.meituan.net/bs/file/?f=fe-sso-fs:build/assets/sp-retina.b95a7dd.png">
        </div>
      </el-col>
      <el-col :span="18">
        <div class="grid-content bg-purple">
          <div class="hasuser">
            <span>已有美团账号？</span>
            <el-button 
              class="login-btn"
              size="mini">登陆</el-button>
          </div>
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
  border-bottom: 2px solid #2dbbaa;
  height: 70px;
}
.header-info {
  width: 1000px;
  margin: 0 auto;
  line-height: 70px;
  height: 70px;
}
.header-info img {
  width: 60px;
  height: 40px;
  box-sizing: border-box;
  vertical-align: middle;
}
.hasuser {
  text-align: right;
}
.hasuser span {
  margin-right: 10px;
  color: #666;
  font-size: 16px;
  line-height: 70px;
  height: 70px;
  vertical-align: middle;
}
.login-btn {
  background-color: #2dbbaa;
  color: #fff;
  height: 30px;
  vertical-align: middle;
}
</style>
