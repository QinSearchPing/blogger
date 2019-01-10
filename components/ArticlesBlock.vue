<template>
  <div class="home-page layout-main">
    <p class="line">
      <!--<span class="title">CODING</span>-->
    </p>
    <ul class="posts-list">
      <li>
        <el-tag type="info">Java</el-tag>
        <a class="title">免费SSL证书升级全站HTTPS</a>
        <span class="createTime">（October 2018）</span>
      </li>
      <li>
        <el-tag type="info">JavaScript</el-tag>
        <a class="title">免费SSL证书升级全站HTTPS</a>
        <span class="createTime">（October 2018）</span>
      </li>
      <li>
        <el-tag type="info">Nodejs</el-tag>
        <a class="title">免费SSL证书升级全站HTTPS</a>
        <span class="createTime">（October 2018）</span>
      </li>
      <li>
        <el-tag type="info">APICloud</el-tag>
        <a class="title">免费SSL证书升级全站HTTPS</a>
        <span class="createTime">（October 2018）</span>
      </li>
      <li>
        <el-tag type="info">Spring</el-tag>
        <a class="title">免费SSL证书升级全站HTTPS</a>
        <span class="createTime">（October 2018）</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'ArticlesBlock'
}
</script>

<style scoped>
.home-page {
  padding: 0 10px;
}
.home-page ul.posts-list {
  margin-bottom: 30px;
  padding: 0 10px;
  list-style: none;
}
.home-page ul.posts-list > li {
  margin-bottom: 10px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

.home-page ul.posts-list > li .title {
  color: #333;
  cursor: pointer;
  text-decoration: underline;
}

.home-page ul.posts-list > li.createTime {
  font-size: 12px;
}
.layout-main {
  min-height: calc(100% - 430px);
  max-width: 640px;
  margin: 0 auto;
  padding-bottom: 20px;
}

.line {
  position: relative;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  margin-bottom: 10px;
}

.line > span.title {
  font-weight: 700;
  padding: 0 10px;
  color: #a7adba;
  background-color: #fff;
}
li {
  display: flex;
  justify-content: space-between;
}
</style>
