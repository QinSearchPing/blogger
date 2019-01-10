<template>
  <div>
    <tags/>
    <div style="margin-top: 50px">
      <articles-block/>
      <articles-block/>
      <articles-block/>
    </div>
  </div>
</template>

<script>
import ArticlesBlock from '@/components/ArticlesBlock'
import Tags from '@/components/Tags'
export default {
  name: 'Articles',
  components: { ArticlesBlock, Tags },
  data() {
    return {
      activeNames: ['1']
    }
  },
  methods: {
    handleChange(val) {
      console.log(val)
    }
  }
}
</script>


<style scoped>
</style>
