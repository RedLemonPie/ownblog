
<template>
  <div class="metro">
    <transition name="bounce">
      <div class="front" @mouseenter="mouseover()" v-show="!showback">
        <slot name="front"></slot>
      </div>
    </transition>
    <transition name="bounce">
      <div class="back" @mouseout="mouseout()" v-if="showback">
        <slot name="back"></slot>
      </div>
    </transition>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showback: false
    }
  },
  components: {},
  mounted() {
    // this.$nextTick(() => {
    //   this.$nuxt.$loading.start()
    //   setTimeout(() => this.$nuxt.$loading.finish(), 500)
    // })
  },
  methods: {
    mouseover() {
      this.showback = true
    },
    mouseout() {
      this.showback = false
    }
  }
}
</script>
<style lang="less" scoped>
.metro {
  width: 180px;
  height: 180px;
  border: 1px solid #000;
  display: flex;
  justify-content: center; /* 水平居中 */
  align-items: center; /* 垂直居中 */
  .front {
    width: 180px;
    height: 180px;
  }
  .back {
    width: 180px;
    height: 180px;
  }
}

.bounce-enter-active {
  animation: bounce-in 0.5s;
}
.bounce-leave-active {
  animation: bounce-in 0.5s reverse;
}
@keyframes bounce-in {
  0% {
    transform: scale(0);
  }
  50% {
    transform: scale(1.5);
  }
  100% {
    transform: scale(1);
  }
}
</style>