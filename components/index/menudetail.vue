<template>
  <div>
    <div class="menudetail">
      <el-tabs 
        v-model="activeName" 
        class="banner"
        @tab-click="handleClick">
        <el-tab-pane 
          label="用户管理" 
          name="first"/>
        <el-tab-pane 
          label="配置管理" 
          name="second"/>
        <el-tab-pane 
          label="角色管理" 
          name="third"/>
        <el-tab-pane 
          label="定时任务补偿" 
          name="fourth"/>
      </el-tabs>
      <div class="banner-info">
        <div class="banner-detail">
          <img src="http://p0.meituan.net/mogu/a8293f59c8d0a5b30241ecbdb13214b650238.jpg">
          <p class="detail-title">千层小姐蛋糕烘焙</p>
          <p class="detail-detail">千层小盒1个，提供免费WiFi</p>
          <p class="detail-info">门市价¥28</p>
        </div>
        <div class="banner-detail">
          <img src="http://p0.meituan.net/mogu/a8293f59c8d0a5b30241ecbdb13214b650238.jpg">
          <p>千层小姐蛋糕烘焙</p>
          <p>千层小盒1个，提供免费WiFi</p>
          <p>门市价¥28</p>
        </div>
        <div class="banner-detail">
          <img src="http://p0.meituan.net/mogu/a8293f59c8d0a5b30241ecbdb13214b650238.jpg">
          <p>千层小姐蛋糕烘焙</p>
          <p>千层小盒1个，提供免费WiFi</p>
          <p>门市价¥28</p>
        </div>
        <div class="banner-detail">
          <img src="http://p0.meituan.net/mogu/a8293f59c8d0a5b30241ecbdb13214b650238.jpg">
          <p>千层小姐蛋糕烘焙</p>
          <p>千层小盒1个，提供免费WiFi</p>
          <p>门市价¥28</p>
        </div>
      </div>  
    </div>
  </div>
</template>
<script>
export default {}
</script>

<style scoped>
.menudetail {
  width: 1200px;
  margin: 0 auto;
  margin-bottom: 20px;
  overflow: hidden;
}
.banner {
  background-color: #bfa97f;
  width: 100%;
  height: 40px;
  padding-left: 20px;
  box-sizing: border-box;
}
.banner-info {
  width: 1200px;
  background-color: #fff;
  padding: 5px;
  box-sizing: border-box;
  overflow: hidden;
}
.banner-detail {
  width: 33.3%;
  height: 350px;
  padding: 10px;
  float: left;
  box-sizing: border-box;
  box-shadow: 2px 2px 5px #999;
}
.banner-detail img {
  width: 100%;
  height: 250px;
}
.detail-title {
  font-size: 16px;
  text-align: left;
}
.detail-detail {
  font-size: 10px;
  color: #999;
  text-align: left;
}
.detail-info {
  color: #bfa97f;
  text-align: left;
  font-size: 16px;
}
</style>
