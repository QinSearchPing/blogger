<template>
  <div>

    <el-menu
      :collapse="isCollapse"
      :router="isRouter"
      default-active="1-4-1"
      class="el-menu-vertical-demo NavMenu"
      @open="handleOpen"
      @close="handleClose">
      <el-menu-item index="/">
        <i class="el-icon-location"/>
        <span slot="title">主页</span>
      </el-menu-item>
      <el-menu-item index="/articles">
        <i class="el-icon-document"/>
        <span slot="title">技术文章</span>
      </el-menu-item>
      <el-menu-item index="/notes">
        <i class="el-icon-edit-outline"/>
        <span slot="title">生活与感悟</span>
      </el-menu-item>
      <el-menu-item index="/note">
        <i class="el-icon-menu"/>
        <span slot="title">相关作品</span>
      </el-menu-item>
      <el-menu-item index="/about">
        <i class="el-icon-info"/>
        <span slot="title">关于我</span>
      </el-menu-item>
      <el-menu-item
        v-if="isCollapse"
        index=""
        @click = "isCollapse = !isCollapse">
        <i class="el-icon-d-arrow-right"/>
        <span slot="title">展开</span>
      </el-menu-item>
      <el-menu-item
        v-if="!isCollapse"
        index=""
        @click = "isCollapse = !isCollapse">
        <i class="el-icon-d-arrow-left"/>
        <span slot="title">收起</span>
      </el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  name: 'NavMenu',
  data() {
    return {
      isCollapse: true,
      isRouter: true
    }
  },
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath)
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath)
    },
    test(event) {
      this.isCollapse = !this.isCollapse
    }
  }
}
</script>

<style scoped>
.NavMenu {
  position: fixed;
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100vh;
}
.el-menu-vertical-demo:not(.el-menu--collapse) {
  width: 200px;
  min-height: 300px;
}
</style>
