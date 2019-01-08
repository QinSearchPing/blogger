<template>
  <div>

    <el-menu
      :collapse="isCollapse"
      default-active="1-4-1"
      class="el-menu-vertical-demo NavMenu"
      @open="handleOpen"
      @close="handleClose">
      <el-menu-item index="1">
        <i class="el-icon-location"/>
        <span slot="title">主页</span>
      </el-menu-item>
      <el-menu-item index="2">
        <i class="el-icon-document"/>
        <span slot="title">全部文章</span>
      </el-menu-item>
      <el-menu-item
        index="3">
        <i class="el-icon-menu"/>
        <span slot="title">技术标签</span>
      </el-menu-item>
      <el-menu-item index="4">
        <i class="el-icon-edit-outline"/>
        <span slot="title">风景与日记</span>
      </el-menu-item>
      <el-menu-item index="5">
        <i class="el-icon-info"/>
        <span slot="title">关于我</span>
      </el-menu-item>
      <el-menu-item
        v-if="isCollapse"
        index="6"
        @click = "isCollapse = !isCollapse">
        <i class="el-icon-d-arrow-right"/>
        <span slot="title">展开</span>
      </el-menu-item>
      <el-menu-item
        v-if="!isCollapse"
        index="6"
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
      isCollapse: true
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
