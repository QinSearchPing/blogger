<template>
  <div
    class="markdown-body"
    v-html="testmd"/>
    <!--</article>-->
</template>

<script>
import testmd from '@/README.md'
export default {
  name: 'Id',
  data() {
    return {
      model: '# Hello World!'
    }
  },
  computed: {
    testmd() {
      return testmd
    }
  }
}
</script>

<style scoped>
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
</style>
