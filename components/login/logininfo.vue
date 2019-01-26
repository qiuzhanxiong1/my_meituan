<template>
  <div class="logininfo">
    <el-row :gutter="0">
      <el-col :span="12">
        <div class="grid-content bg-purple loginimg">
          <img src="http://s0.meituan.net/bs/file/?f=fe-sso-fs:build/page/static/banner/www.jpg">
        </div>
      </el-col>
      <el-col :span="12">
        <div class="grid-content bg-purple">
          <div class="logindetail">
            <div class="loginerror"><span>请输入账号和密码</span></div>
            <p class="username">账号登录</p>
            <el-input 
              v-model="user_name" 
              placeholder="请输入内容"
              class="login-input"/>
            <el-input 
              v-model="user_psd" 
              placeholder="请输入内容"
              class="login-input"/>
            <p class="lostpsd">忘记密码？</p>
            <el-button class="login-btn">登陆</el-button>
            <p class="nouser">还没有账号？<span>免费注册</span></p>
            <p class="otheruser">用合作网站账号登录</p>
          </div>
        </div>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  data() {
    return {
      user_name: '',
      user_psd: ''
    }
  }
}
</script>
<style scoped>
.logininfo {
  width: 1000px;
  margin: 0 auto;
  padding-bottom: 50px;
}
.loginimg {
  padding: 20px;
}
.logindetail {
  width: 300px;
  margin: 0 auto;
}
.loginerror,
.login-input {
  width: 270px;
  height: 36px;
  line-height: 36px;
  margin-top: 15px;
}
.login-input {
  margin-top: 5px;
}
.login-input + .login-input {
  margin-top: 20px;
}
.loginerror {
  background-color: #fff6db;
  border: 1px solid #f5d8a7;
}
.loginerror span {
  margin-left: 30px;
}
.login-btn {
  width: 270px;
  height: 36px;
  background-color: #2dbbaa;
  text-align: center;
  line-height: 6px;
  margin-top: 5px;
}
.login-btn span {
  font-size: 16px;
}
.logindetail {
  padding: 5px;
}
.username {
  height: 20px;
  line-height: 20px;
  font-size: 14px;
  color: #999;
  margin-top: 10px;
}
.lostpsd {
  color: #2dbbaa;
  text-align: right;
  margin-top: 15px;
  width: 270px;
}
.nouser {
  font-size: 14px;
  color: #999;
  margin-top: 5px;
}
.nouser span {
  color: #2dbbaa;
}
.otheruser {
  margin-top: 10px;
  font-size: 14px;
  color: #999;
  text-align: center;
  width: 270px;
}
</style>
