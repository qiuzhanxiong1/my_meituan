<template>
  <div>
    <el-row :gutter="0">
      <el-col :span="24">
        <div class="grid-content bg-purple">
          <login-header/>
        </div>
      </el-col>
    </el-row>
    <el-row :gutter="0">
      <el-col :span="24">
        <div class="grid-content bg-purple">
          <login-info/>
        </div>
      </el-col>
    </el-row>
    <el-row :gutter="0">
      <el-col :span="24">
        <div class="grid-content bg-purple">
          <login-footer/>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import LoginHeader from '../components/login/loginheader'
import LoginInfo from '../components/login/logininfo'
import LoginFooter from '../components/login/loginfooter'
export default {
  layout: 'black',
  components: {
    LoginHeader,
    LoginInfo,
    LoginFooter
  }
}
</script>

<style scoped>
</style>
