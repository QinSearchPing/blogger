<template>
  <article>
    <header style="border-bottom: none">
      <h1 class="post-title">
        <a
          href=""
          class="post-title-link">博客标题List</a>
      </h1>
      <div class="post-meta">
        <span>
          <span>发表于</span>
          <time>2018-12-04</time>
        </span>
        <span>
          &nbsp;| &nbsp;
          <span>作者：Uranus</span>
        </span>
        <!--<span>作者 杨汉钦</span>-->
      </div>
      <div/>
    </header>
    <div>
      开发代码兼容Vue CLI 3初始化的项目，构建时会根据package.json中的browserslist配置自动检测需要转译的语言特性，为构建代码转译JavaScript 并为 CSS 添加浏览器前缀，通常只需要修改browserslist即可兼容目标浏览器，例如兼容IE10可以做如下配置： 1，
      <div class="post-more-link text-center">
        <a
          href=""
          class="btn">阅读全文 >></a>
      </div>
    </div>
    <footer class="post-footer">
      <div class="post-eof"/>
    </footer>
  </article>
</template>
<script>
export default {
  name: 'ArticleAbstract'
}
</script>

<style scoped>
article {
  font-size: 18px;
  line-height: 2;
  color: #555;
}
a {
  text-decoration: none;
}
.post-title {
  font-size: 26px;
  text-align: center;
  font-weight: 400;
}
.post-title-link {
  display: inline-block;
  position: relative;
  color: #555;
  border-bottom: none;
  line-height: 1.2;
  vertical-align: top;
}
.post-meta {
  margin: 3px 0 40px 0;
  color: #999;
  font-size: 12px;
  text-align: center;
}

.post-more-link {
  margin-top: 50px;
}
.text-center {
  text-align: center;
}
.post-eof {
  isplay: block;
  margin: 80px auto 60px;
  width: 8%;
  height: 1px;
  background: #ccc;
  text-align: center;
}

.btn {
  display: inline-block;
  padding: 0 20px;
  font-size: 14px;
  color: #fff;
  background: #222;
  border: 2px solid #222;
  text-decoration: none;
  border-radius: 0;
  transition-property: background-color;
  transition-duration: 0.2s;
  transition-timing-function: ease-in-out;
  transition-delay: 0s;
}
</style>
