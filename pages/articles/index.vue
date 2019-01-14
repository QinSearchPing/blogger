<template>
  <div>
    <tags/>
    <div style="margin-top: 50px">
      <articles-block :articles="articleList"/>
    </div>
  </div>
</template>

<script>
import ArticlesBlock from '@/components/ArticlesBlock'
import Tags from '@/components/Tags'
export default {
  name: 'Articles',
  components: { ArticlesBlock, Tags },
  data: function() {
    return {
      articleList: [
        {
          id: '001',
          tag: 'Java',
          title: '博客标题',
          time: '2018-12-04',
          author: 'Uranus',
          content:
            '开发代码兼容Vue CLI 3初始化的项目，构建时会根据package.json中的browserslist配置自动检测需要转译的语言特性，为构建代码转译JavaScript 并为 CSS 添加浏览器前缀，通常只需要修改browserslist即可兼容目标浏览器，例如兼容IE10可以做如下配置'
        },
        {
          id: '002',
          tag: 'Java',
          title: '博客标题',
          time: '2018-12-04',
          author: 'Uranus',
          content:
            '开发代码兼容Vue CLI 3初始化的项目，构建时会根据package.json中的browserslist配置自动检测需要转译的语言特性，为构建代码转译JavaScript 并为 CSS 添加浏览器前缀，通常只需要修改browserslist即可兼容目标浏览器，例如兼容IE10可以做如下配置'
        }
      ]
    }
  }
}
</script>


<style scoped>
</style>
