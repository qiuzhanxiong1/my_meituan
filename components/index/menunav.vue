<template>
  <div class="menu-nav">
    <dl>
      <dt>全部分类</dt>
      <dd>
        <i class=" food"/>美食
        <span>></span>
      </dd>
    </dl>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.menu-nav {
  width: 100%;
  position: relative;
  font-family: 'iconfont';
}
.menu-nav dl {
  height: 475px;
  position: relative;
  box-sizing: border-box;
  background: linear-gradient(
    to bottom,
    rgba(2, 181, 157, 0.85) 2%,
    rgba(22, 146, 183, 0.85) 100%
  );
  top: -50px;
  color: #fff;
}
.menu-nav dl dt {
  height: 50px;
  line-height: 50px;
  font-size: 16px;
  text-align: left;
  padding-left: 20px;
}
.menu-nav dl dd {
  height: 25px;
  line-height: 25px;
  text-align: left;
  padding-left: 20px;
}
.menu-nav dl dd:hover {
  background-color: rgba(255, 255, 255, 0.2);
}
.menu-nav dl dd span {
  margin-left: 180px;
}
.food {
  content: '\e622';
}
.takeout {
  content: '\e630';
}
.hotel {
  content: '\e62a';
}
.homestay {
  content: '\e631';
}
.movie {
  content: '\e62c';
}
.airport {
  content: '\e632';
}
.ktv {
  content: '\e627';
}
.life {
  content: '\e633';
}
.hair {
  content: '\e626';
  transform: scale(0.7);
}
.marry {
  content: '\e629';
}
.offspring {
  content: '\e623';
}
.sport {
  content: '\e62b';
}
.furniture {
  content: '\e625';
}
.study {
  content: '\e624';
}
.health {
  content: '\e628';
}
.bar {
  content: '\e621';
}
</style>
