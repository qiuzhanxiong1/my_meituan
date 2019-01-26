<template>
  <div class="footer">
    <ul class="clearfloat">
      <li>关于美团</li>
      <li>加入我们</li>
      <li>商家入驻</li>
      <li>帮助中心</li>
      <li>美团手机版</li>
    </ul>
  </div>
</template>

<script>
export default {}
</script>
<style scoped>
.footer {
  width: 1000px;
  margin: 0 auto;
  padding: 20px;
}
.footer ul {
  margin-left: -20px;
}
.footer li {
  float: left;
  color: #999;
  width: 70px;
  padding: 0px 20px;
  text-align: center;
}
.footer li + li {
  border-left: 1px solid #999;
}
</style>
