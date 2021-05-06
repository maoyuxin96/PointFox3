<template>
  <div id="RegisterWrapper">
    <div id="mainContent">
      <el-card class="box-card">
        <div slot="header" class="clearfix">
          <span>用户注册</span>
          
        </div>
        <div id="RegisterContent">
          <el-input id="username" v-model="newUser.username" clearable></el-input>
          <el-input id="password" v-model="newUser.password" show-password></el-input>
        </div>
        <div id="submitContent">
          <el-button id="SystemSubmit">注册</el-button>
        </div>
      </el-card>
    </div>
  </div>
</template>

<script>
export default {
 data(){
    return{
      newUser:{
        username:"",
        password:""
      }
    }
  }
};

</script>

<style>
#RegisterWrapper {
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