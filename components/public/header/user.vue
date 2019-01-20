<template>
  <div class="hearder-user">
    <div v-if="!is_login">
      <nuxt-link to="/">立即登录</nuxt-link>
      <nuxt-link to="/">注册</nuxt-link>
    </div>
    <div v-if="is_login">
      <div>用户名</div>
      <nuxt-link to="/">退出登陆</nuxt-link>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      is_login: ''
    }
  }
}
</script>
<style scoped>
</style>
