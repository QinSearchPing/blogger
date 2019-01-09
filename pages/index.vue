<template>
  <div>
    <article-abstract/>
    <article-abstract/>
    <!--<article-abstract/>-->
  </div>
</template>

<script>
import ArticleAbstract from '~/components/ArticleAbstract.vue'
export default {
  components: {
    ArticleAbstract
  }
}
</script>

<style>
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
  text-align: center;
  line-height: 160px;
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
