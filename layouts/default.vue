<template>
  <div>
    <el-container style="height: 100vh">
      <nav-menu class="nav-menu-structure"/>
      <el-container>
        <el-header class="el-header-structure">
          <info-header/>
        </el-header>
        <el-main class="el-main-structure">
          <nuxt/>
        </el-main>
        <el-footer style="height: 5vh">
          <info-footer/>
        </el-footer>
      </el-container>
    </el-container>

  </div>
</template>
<script>
import NavMenu from '~/components/NavMenu.vue'
import InfoHeader from '~/components/Header.vue'
import InfoFooter from '~/components/Footer.vue'
import ArticleAbstract from '~/components/ArticleAbstract.vue'

export default {
  components: {
    NavMenu,
    InfoHeader,
    InfoFooter,
    ArticleAbstract
  }
}
</script>
<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.nav-menu-structure {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.el-header-structure {
  height: 35vh;
  min-width: 800px;
  min-height: 300px;
}
.el-main-structure {
  margin: 0 auto;
  width: 800px;
}
.el-header,
.el-footer {
  color: #333;
  text-align: center;
  /*line-height: 60px;*/
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 500px;
  width: 20vh;
}

.el-main {
  color: #333;
  /*text-align: center;*/
  /*line-height: 160px;*/
  overflow: initial;
  padding: 60px 20px 20px;
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
