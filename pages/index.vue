<template>
  <div class= "main">
    <Firstscreen></Firstscreen>

    <div class="container"><nuxt-link to="/blog">进入首页</nuxt-link></div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Firstscreen from '~/components/Firstscreen'

export default {
  components: {
    Logo,
    Firstscreen
  },
  mounted () {
    // this.$nextTick(() => {
    //   this.$nuxt.$loading.start()
    //   setTimeout(() => this.$nuxt.$loading.finish(), 500)
    // })
  }
}
</script>

<style lang="less" scope="scope">
.main{
  height: 100%;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
