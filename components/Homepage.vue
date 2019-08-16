
<template>
  <div class="container">
    <!-- <nuxt-link to="/blog">进入首页</nuxt-link> -->
    <Metrobox>
      <template #front>
        <div>简介</div>
      </template>
      <template #back>
        <div>你,必须点</div>
      </template>
    </Metrobox>
    <Metrobox>
      <div>111111</div>
    </Metrobox>
    <Metrobox>
      <div>111111</div>
    </Metrobox>
  </div>
</template>
<script>
import Metrobox from '~/components/Metrobox.vue'

export default {
  components: {
    Metrobox
  },
  mounted() {
    // this.$nextTick(() => {
    //   this.$nuxt.$loading.start()
    //   setTimeout(() => this.$nuxt.$loading.finish(), 500)
    // })
  }
}
</script>
<style lang="less" scoped>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>