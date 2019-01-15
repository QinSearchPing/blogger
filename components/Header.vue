<template>
  <div class="header">
    <img
      src="@/assets/images/identify.jpg"
      alt="avatar"
      class="avatar">
    <p class="site-subtitle">自先沉稳 而后爱人</p>
    <nav>
      <ul class="menu">
        <li class="menu-item">
          <nuxt-link to="/">
            <i class="el-icon-location"><br>主页</i>
          </nuxt-link>
        </li>
        <li class="menu-item">
          <nuxt-link to="/articles">
            <i class="el-icon-document" ><br>技术文章</i>
          </nuxt-link>
        </li>
        <li class="menu-item">
          <nuxt-link to="/notes">
            <i class="el-icon-edit-outline" ><br>生活与感悟</i>
          </nuxt-link>
        </li>
        <li class="menu-item">
          <nuxt-link to="/projects">
            <i class="el-icon-menu" ><br>相关作品</i>
          </nuxt-link>
        </li>
        <li class="menu-item">
          <nuxt-link to="/about">
            <i class="el-icon-info" ><br>关于我</i>
          </nuxt-link>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      radio: '1'
    }
  }
}
</script>

<style scoped>
.header {
  margin: 50px;
  line-height: 2;
  font-size: 14px;
}
.avatar {
  margin: 0 auto;
  width: 128px;
  height: 128px;
  border-radius: 50%;
  opacity: 0.6;
}
.site-subtitle {
  margin-top: 5px;
  font-size: 13px;
  color: #999;
}

.menu {
  margin-top: 20px;
  padding-left: 0;
  text-align: center;
}
.menu .menu-item {
  display: inline-block;
  margin: 0 10px;
}
.menu .menu-item a {
  display: block;
  font-size: 13px;
  text-transform: capitalize;
  line-height: inherit;
  border-bottom: 1px solid transparent;
  transition-property: border-color;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
  transition-delay: 0s;
}
i {
  line-height: 2;
  color: #555;
}
</style>
