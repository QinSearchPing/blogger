<template>
  <article>
    <header style="border-bottom: none">
      <h1 class="post-title">
        <a
          href=""
          class="post-title-link">{{ article.title }}</a>
      </h1>
      <div class="post-meta">
        <span>
          <span>发表于</span>
          <time>{{ article.time }}</time>
        </span>
        <span>
          &nbsp;| &nbsp;
          <span>作者：{{ article.author + article.id }} </span>
        </span>
        <!--<span>作者 杨汉钦</span>-->
      </div>
      <div/>
    </header>
    <div>
      {{ article.content }}
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
  name: 'ArticleAbstract',
  props: {
    article: {
      type: Object,
      required: true,
      default: function() {
        return {
          id: '',
          title: '',
          time: '',
          author: '',
          content: ''
        }
      }
    }
  }
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
