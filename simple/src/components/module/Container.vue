
<template>
  <el-container style="height: 800px; border: 1px solid #eee">
    <el-header>Header</el-header>
    <el-container>
      <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
        <Menu/>
      </el-aside>
      <el-main>    
       <router-view></router-view> 
      </el-main>
    </el-container>
    <!-- <el-footer>Footer</el-footer> -->
  </el-container>
</template>
<script>
import Menu from "./Menu";
import Table from './Table'
export default {
  name: "main",
  components: {
    Menu,
    Table
  }
};
</script>
<style>
.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
  text-align: center;
  line-height: 60px;
}
.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 200px;
}
.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}
body > .el-container {
  margin-bottom: 40px;
}
.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}
.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
