<template>
  <div class="register">
    <el-form
      ref="ruleForm"
      :model="ruleForm"
      :rules="rules"
      label-width="100px"
      class="demo-ruleForm"
    >
      <el-form-item 
        label="手机号" 
        prop="phone">
        <el-input 
          v-model="ruleForm.phone" 
          class="btn"/>
      </el-form-item>
      <el-form-item 
        label="邮箱" 
        prop="email">
        <el-input 
          v-model="ruleForm.email" 
          class="btn"/>
      </el-form-item>
      <el-form-item 
        label="创建密码" 
        prop="psd">
        <el-input 
          v-model="ruleForm.psd" 
          class="btn"/>
      </el-form-item>
      <el-form-item 
        label="确认密码" 
        prop="repsd">
        <el-input 
          v-model="ruleForm.repsd" 
          class="btn"/>
      </el-form-item>
      <el-form-item>
        <el-button 
          type="primary" 
          class="submit" 
          @click="submitForm('ruleForm')">同意以下协议并注册</el-button>
        <el-button @click="resetForm('ruleForm')">重置</el-button>
        <div class="rule">《美团网用户协议》</div>
      </el-form-item>
    </el-form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      ruleForm: {
        phone: '',
        email: '',
        psd: '',
        repsd: ''
      },
      rules: {
        phone: [
          {
            required: true,
            type: 'string',
            message: '请输入手机号码',
            trigger: 'blur'
          }
        ],
        email: [
          {
            required: true,
            type: 'email',
            message: '请输入邮箱',
            trigger: 'blur'
          }
        ],
        psd: [
          {
            required: true,
            message: '创建密码',
            trigger: 'blur'
          }
        ],
        repsd: [
          {
            required: true,
            message: '确认密码',
            trigger: 'blur'
          }
        ]
      }
    }
  },
  methods: {
    submitForm(formName) {
      this.$refs[formName].validate(valid => {
        if (valid) {
          alert('submit!')
        } else {
          console.log('error submit!!')
          return false
        }
      })
    },
    resetForm(formName) {
      this.$refs[formName].resetFields()
    }
  }
}
</script>
<style scoped>
.register {
  width: 1000px;
  margin: 40px auto 0px;
}
.btn {
  width: 300px;
}
.rule {
  color: #2dbbaa;
  font-weight: bold;
}
.submit {
  background-color: #2dbbaa;
}
</style>
