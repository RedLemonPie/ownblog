<template>
  <div class= "main">
    <Firstscreen></Firstscreen>
    <Homepage> </Homepage>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Firstscreen from '~/components/Firstscreen'
import Homepage from '~/components/Homepage'

export default {
  components: {
    Logo,
    Firstscreen,
    Homepage
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
</style>
