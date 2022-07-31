<template>
  <div class="login">
    <!-- 表单居中大盒子 -->
    <div class="form">
      <!-- 帝可得图片 -->
      <div>
        <img class="logo" src="../../assets/logo.595745bd.png" alt="" />
      </div>
      <!-- 表单框盒子 -->
      <div class="formSon">
        <el-form ref="form" :model="form" >
          <el-form-item>
            <el-input
              placeholder="请输入账号"
              prefix-icon="el-icon-mobile-phone"
            ></el-input>
          </el-form-item>
          <el-form-item>
            <el-input
              placeholder="请输入密码"
              prefix-icon="el-icon-lock"
              suffix-icon="iconfont icon-yanjing"
            ></el-input> </el-form-item
          ><el-form-item>
            <el-input
              placeholder="请输入验证码"
              prefix-icon="el-icon-price-tag"
            ></el-input>
            <img class="CAPTCHA" src="../../assets/2EB9ORVshCyds3l7C78KrTc6CqEgHJ4N.jpeg" alt="">
          </el-form-item>
          <el-form-item>
            <el-button type="primary">登录</el-button>
          </el-form-item>
        </el-form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        name: '',
        region: '',
        date1: '',
        date2: '',
        delivery: false,
        type: [],
        resource: '',
        desc: '',
      },
    }
  },
  methods: {},

  mounted() {},

  created() {},

  components: {},

  computed: {},
}
</script>

<style lang="less">
* {
  margin: 0;
  padding: 0;
}
.login {
  width: 100vw;
  height: 100vh;
  background: url('../../assets/background.be4fae7d.png');
  background-size: cover;
}
.form {
  margin: 0 auto;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 518px;
  height: 388px;
  background: #fff;
  border-radius: 10px;
}
.logo {
  width: 96px;
  height: 96px;
  position: relative;
  top: -45px;
  left: 210px;
}
.CAPTCHA{
  width: 130px;
  height: 50px;
}
.formSon {
  // background-color: pink;
  width: 448px;
  height: 280px;
  margin: 8px auto 0;
}
input {
  margin: 0 auto;
  border:unset
  
}
.el-input__inner{
height:50px;
}
// .el-input{
//   // border:1px solid #e2e2e2

// }
.el-icon-mobile-phone:before {
  position: relative;
  top: 0;
  left: 0;
}
// 按钮颜色
button {
  width: 100%;
  height: 52px;
  background: linear-gradient(262deg, #2e50e1, #6878f0);
  opacity: 0.91;
  border-radius: 8px;
  color: #fff;
}
.el-form-item__content{
  display: flex;
}
</style>
