<template>
  <div id="mainwrapper">
    <div id="mainContent">
      <el-card class="box-card">
        <div slot="header" class="clearfix">
          <span>系统登录</span>
          <el-button style="float: right; padding: 3px 0" type="text"
          > 忘记密码</el-button>
        </div>
        <div id="loginContent">
          <el-input id="username" v-model="user.username" clearable></el-input>
          <el-input id="password" v-model="user.password" show-password></el-input>
        </div>
        <div id="submitContent">
          <el-button id="SystemSubmit">登录</el-button>
        </div>
      </el-card>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      user:{
        username:"",
        password:""
      }
    }
  }
};
</script>

<style>
#mainwrapper {
  /* background-color: pink; */
  padding-top: 90px;
}
#mainContent{
  width: 400px;
  margin: 0 auto;
}
#SystemSubmit{
  background-color: #0a9588 !important;
    border-color: #0a9588 !important;
    color: white  !important;
    margin: 0 auto;
    display:block;
}
#password{
  margin: 5px 0;
}
</style>