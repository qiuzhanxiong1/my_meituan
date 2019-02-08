<template>
  <div>
    <el-row :gutter="0">
      <el-col :span="24">
        <div class="grid-content bg-purple">
          <register-header/>
        </div>
      </el-col>
    </el-row>
    <el-row :gutter="0">
      <el-col :span="24">
        <div class="grid-content bg-purple">
          <register-info/>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import RegisterHeader from '../components/register/header'
import RegisterInfo from '../components/register/registerinfo'
export default {
  layout: 'black',
  components: {
    RegisterHeader,
    RegisterInfo
  }
}
</script>
<style scoped>
</style>
