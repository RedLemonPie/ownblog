<template>
  <div class="firstscreen">
    <div class="name">RedLemonPie</div>
    <div class="description">Different But One World</div>
    <div class="enter">欢迎哦</div>
  </div>
</template>

<style lang="less" scoped>
.firstscreen {
  background: rgb(199, 199, 199);
  background: radial-gradient(rgb(0, 0, 0), rgb(70, 70, 70));
  width: 100%;
  height: 100%;
  margin: 0 auto;
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
  flex-wrap: wrap;
  color: white;
  .name {
    padding-top: 30vh;
    text-shadow: 0px 0px 20px rgb(255, 255, 255);
    font-size: 120px;
  }
  .description {
    width: 100%;
    font-size: 2vw;
    // font-size: 2rem;
  }
  .enter {
    width: 100%;
    padding-top: 10vh;
    font-size: 2vw;
    // font-size: 2rem;
  }
}
</style>