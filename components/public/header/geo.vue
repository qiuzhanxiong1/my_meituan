<template>
  <div class="m-geo clearfloat">
    <i class="el-icon-location"/>
    <div>嘉兴</div>
    <nuxt-link to="/">切换城市</nuxt-link>
    [ 嘉善 桐乡 海宁]
  </div>
</template>
<script>
export default {}
</script>
<style scoped>
.m-geo i,
.m-geo div,
.m-geo nuxt-link {
  float: left;
}
i {
  display: block;
  height: 40px;
  line-height: 40px;
  width: 20px;
}
</style>
