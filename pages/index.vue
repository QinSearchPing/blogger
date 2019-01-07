<template>
  <div>
    <el-container style="height: 100vh">
      <!--<el-aside>-->
      <nav-menu style="display: flex;flex-direction: column;justify-content: center"/>
      <!--</el-aside>-->
      <el-container>
        <el-header>Header</el-header>
        <el-main>main</el-main>
        <el-footer>Footer</el-footer>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import NavMenu from '~/components/NavMenu.vue'
export default {
  components: {
    Logo,
    NavMenu
  }
}
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
  line-height: 500px;
  width: 20vh;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}

body > .el-container {
  margin-bottom: 40px;
  height: 100vh;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
