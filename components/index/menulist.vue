<template>
  <div class="menu">
    <el-row 
      :gutter="20" 
      class="menutop"
      style="margin-left:0;margin-right:0;">
      <el-col :span="14">
        <div class="block swiper">
          <el-carousel height="240px">
            <el-carousel-item>
              <img src="http://p0.meituan.net/codeman/daa73310c9e57454dc97f0146640fd9f69772.jpg">
            </el-carousel-item>
            <el-carousel-item>
              <img src="http://p1.meituan.net/codeman/826a5ed09dab49af658c34624d75491861404.jpg">
            </el-carousel-item>
            <el-carousel-item>
              <img src="http://p0.meituan.net/codeman/a97baf515235f4c5a2b1323a741e577185048.jpg">
            </el-carousel-item>
          </el-carousel>
        </div>  
      </el-col>
      <el-col :span="4">
        <div class="menulist1">
          <img src="http://p0.meituan.net/codeman/e473bb428f070321269b23370ff02ba956209.jpg">  
        </div>
      </el-col>
      <el-col :span="6">
        <div class="login">
          <div class="login-img">1</div>
          <div class="login-title">Hi！你好</div>
          <div >
            <el-button
              round
              class="login-btn">注册</el-button>
          </div>
          <div >
            <el-button
              round
              class="login-btn">立即登陆</el-button>
          </div>
        </div>  
      </el-col>
    </el-row>
    <el-row 
      :gutter="20"
      class="menubottom" 
      style="margin-left:0;margin-right:0;">
      <el-col 
        :span="7">
        <div class="menulist2">
          <img src="http://p1.meituan.net/codeman/8cce56c467a17e04f3094d1e455462a0132772.png">  
        </div>
      </el-col>
      <el-col 
        :span="7">
        <div class="menulist2">
          <img src="http://p1.meituan.net/codeman/16442c19da1f1c4544f794e29d99c92051716.jpg">
        </div>  
      </el-col>
      <el-col :span="4">
        <div class="menulist3">
          <img src="http://p1.meituan.net/codeman/5b21cddb4bb1cbc3a9c3bce0f726c75940469.jpg">  
        </div>  
      </el-col>
      <el-col :span="6">
        <div class="app-icon">
          <div class="app-iconfont">
            <img src="http://s1.meituan.net/bs/fe-web-meituan/60ac9a0/img/download-qr.png">
          </div>
          <div>美团APP手机版</div>
          <div><span>1元起</span>吃喝玩乐</div>  
        </div>  
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.menutop {
  margin-top: 15px;
}
.swiper {
  height: 240px;
  position: relative;
  z-index: 0;
}
.menulist1 {
  height: 240px;
  width: 150px;
  margin-left: -10px;
}
.el-col-pad {
  padding: 0;
}
.login {
  background-color: #fff;
  height: 240px;
  border: 1px solid transparent;
  box-sizing: border-box;
  margin-left: -10px;
}
.login-img {
  margin-top: 30px;
}
.login-title {
  margin-top: 20px;
  font-size: 20px;
}
.login-btn {
  margin-top: 20px;
  width: 120px;
}
.menubottom {
  margin-top: 10px;
}
.menulist2 {
  height: 160px;
  width: 100%;
}
.menulist3 {
  height: 160px;
  width: 150px;
  margin-left: -10px;
}
.app-icon {
  height: 160px;
  background-color: #fff;
  box-sizing: border-box;
  margin-left: -10px;
}
.app-iconfont {
  height: 100px;
  width: 100px;
  margin: 0 auto;
}
img {
  height: 100%;
  width: 100%;
}
</style>
