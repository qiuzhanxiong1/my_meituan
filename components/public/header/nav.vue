<template>
  <div class="header-nav">
    <ul>
      <li 
        @mouseover="openmy" 
        @mouseleave="closemy">
        <nuxt-link to="/">我的美团</nuxt-link>
        <dl 
          v-show="showmy"
          class="my">
          <dd><nuxt-link to="/dingdan">我的订单</nuxt-link></dd>
          <dd>我的收藏</dd>
          <dd>抵用券</dd>
          <dd>账户设置</dd>
        </dl>
      </li>
      <li>手机APP</li>
      <li 
        @mouseover="openshop" 
        @mouseleave="closeshop">
        <nuxt-link to="/">商家中心</nuxt-link>
        <dl 
          v-show="showshop"
          class="shopcenter">
          <dd><nuxt-link to="/">登陆商家中心</nuxt-link></dd>
          <dd>美团智能收银</dd>
          <dd>我想合作</dd>
          <dd>手机免费开店</dd>
        </dl>
      </li>
      <li
        @mouseover="openbanner" 
        @mouseleave="closebanner">
        <span>网站导航</span>
        <div 
          v-show="showbanner"
          class="banner">
          <dl class="hotel">
            <dt>酒店旅游</dt>
            <dd>国际机票</dd>
            <dd>国际机票</dd>
            <dd>国际机票</dd>
            <dd>国际机票</dd>
          </dl>
          <dl class="food">
            <dt>吃美食</dt>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
            <dd>烤鱼</dd>
          </dl>
          <dl class="movie">
            <dt>看电影</dt>
            <dd>热映电影</dd>
          </dl>
          <dl class="app">
            <dt>手机应用</dt>
            <dd>
              <img src="http://s0.meituan.net/bs/fe-web-meituan/e5eeaef/img/appicons/meituan.png" >
            </dd>
            <dd>
              <img src="http://s1.meituan.net/bs/fe-web-meituan/404d350/img/appicons/waimai.png" >
            </dd>
            <dd>
              <img src="http://s0.meituan.net/bs/fe-web-meituan/404d350/img/appicons/zhenguo.png" >
            </dd>
            <dd>
              <img src="http://s1.meituan.net/bs/fe-web-meituan/404d350/img/appicons/dianping.png" >
            </dd>
            <dd>
              <img src="http://s1.meituan.net/bs/fe-web-meituan/404d350/img/appicons/maoyan.png" >
            </dd>
          </dl>
        </div>
      </li>
    </ul>  
  </div>
</template>
<script>
export default {
  data() {
    return {
      showmy: false,
      showshop: false,
      showbanner: false
    }
  },
  methods: {
    openmy() {
      this.showmy = true
    },
    closemy() {
      this.showmy = false
    },
    closeshop() {
      this.showshop = false
    },
    openshop() {
      this.showshop = true
    },
    openbanner() {
      this.showbanner = true
    },
    closebanner() {
      this.showbanner = false
    }
  }
}
</script>
<style scoped>
.header-nav {
  float: right;
  width: 350px;
}
.header-nav ul li {
  float: left;
  width: 80px;
  margin-right: 5px;
  box-sizing: border-box;
  position: relative;
  z-index: 1;
}
.header-nav ul li:nth-child(1):hover,
.header-nav ul li:nth-child(4):hover {
  background-color: #fff;
  border-left: 1px solid transparent;
  border-right: 1px solid transparent;
  box-shadow: 0 3px 5px 0 rgba(0, 0, 0, 0.1);
}
.header-nav ul li:nth-child(3):hover {
  background-color: #fff;
  border-left: 1px solid transparent;
  border-right: 1px solid transparent;
  border-bottom: 1px solid transparent;
  box-shadow: 0 -2px 3px 0 rgba(0, 0, 0, 0.1);
}
.my {
  width: 80px;
  position: absolute;
  border: 1px solid #e5e5e5;
  border-top: 1px solid transparent;
  box-shadow: 0 3px 5px 1px rgba(0, 0, 0, 0.1);
  top: 40px;
  left: -2px;
  z-index: 100;
  background-color: #fff;
}
.shopcenter {
  width: 100px;
  border: 1px solid #e5e5e5;
  border-top: 1px solid transparent;
  box-shadow: 0 3px 5px 1px rgba(0, 0, 0, 0.1);
  position: absolute;
  left: -22px;
  top: 40px;
  z-index: 1000;
}
.banner {
  width: 1200px;
  border-top: 1px solid transparent;
  box-shadow: 0 3px 5px 1px rgba(0, 0, 0, 0.1);
  position: absolute;
  left: -1121px;
  height: 300px;
  z-index: 1000;
  background-color: #fff;
}
.banner dl {
  float: left;
  text-align: center;
  box-sizing: border-box;
}
.hotel {
  width: 30%;
  padding: 0 50px;
}
.hotel dd {
  width: 33%;
  float: left;
  text-align: center;
}
.food {
  width: 15%;
  padding: 0 20px;
}
.food dd {
  width: 50%;
  float: left;
  text-align: center;
}
.movie {
  width: 10%;
}
.app {
  width: 40%;
  padding: 0 70px;
}
.app dd {
  float: left;
  width: 17%;
}
.app dd + dd {
  margin-left: 12px;
}
.app dd img {
  width: 100%;
  height: 100%;
}
.banner dl dt {
  height: 100px;
  line-height: 100px;
  text-align: center;
  color: #31bbac;
  font-size: 18px;
}
</style>
