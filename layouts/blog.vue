<template>
  <a-layout id="components-layout-demo-side" style="min-height: 100vh">
    <a-layout-sider collapsible v-model="collapsed">
      <div class="logo" />
      <!-- <side-menu></side-menu> -->
    </a-layout-sider>
    <a-layout>
      <!-- <a-layout-header style="background: #fff; padding: 0" /> -->
      <a-layout-content style="margin: 0 16px">
        <no-ssr>
          <vue-particles
            color="#dfcddf"
            :particleOpacity="0.7"
            :particlesNumber="60"
            shapeType="circle"
            :particleSize="4"
            linesColor="#ce1233"
            :linesWidth="1"
            :lineLinked="true"
            :lineOpacity="0.4"
            :linesDistance="150"
            :moveSpeed="2"
            :hoverEffect="true"
            hoverMode="repulse"
            :clickEffect="false"
            clickMode="push"
            class="lizi"
          ></vue-particles>
        </no-ssr>
        <nuxt />
      </a-layout-content>
      <!-- <a-layout-footer style="text-align: center">
        Ant Design ©2018 Created by Ant UED
      </a-layout-footer>-->
    </a-layout>
  </a-layout>
</template>


<script>
export default {
  components: {
  },
  mounted() {
    // this.$nextTick(() => {
    //   this.$nuxt.$loading.start()
    //   setTimeout(() => this.$nuxt.$loading.finish(), 500)
    // })
  }
}
</script>

<style>
</style>
