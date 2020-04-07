<template>
  <div class="base-header">
    <div class="container">
      <div class="base-header__top">
        <header>
          <div class="base-header__logo">
            <img class="base-header__logo-logo" alt="mzl logo" src="../assets/logo.png">        
            <p class="base-header__logo__desc">
              <span>书山有路勤为径，学海无涯苦作舟</span>
              <ship-icon :style="{ fontSize: '32px' }" />
            </p>
          </div>
        </header>
        <nav class="base-header__nav">
          <router-link to="/">首页</router-link> |
          <router-link to="/about">联系</router-link>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
const svgShip = {
  template:`
  <svg t="1586253217699" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2475" width="200" height="200"><path d="M618.666667 576H106.666667s21.333333 0 42.666666 64 42.666667 128 149.333334 128c42.666667 0 298.666667 21.333333 384 21.333333 104.213333 0 137.728-155.498667 204.117333-213.333333H618.666667z" fill="#795548" p-id="2476"></path><path d="M938.666667 725.333333c-64 0-85.333333-42.666667-85.333334-42.666666s-21.333333 42.666667-85.333333 42.666666-85.333333-42.666667-85.333333-42.666666-21.333333 42.666667-85.333334 42.666666-85.333333-42.666667-85.333333-42.666666-21.333333 42.666667-85.333333 42.666666-85.333333-42.666667-85.333334-42.666666-21.333333 42.666667-85.333333 42.666666-85.333333-42.666667-85.333333-42.666666-21.333333 42.666667-85.333334 42.666666v170.666667h853.333334v-170.666667z" fill="#90CAF9" p-id="2477"></path><path d="M938.666667 810.666667c-64 0-85.333333-42.666667-85.333334-42.666667s-21.333333 42.666667-85.333333 42.666667-85.333333-42.666667-85.333333-42.666667-21.333333 42.666667-85.333334 42.666667-85.333333-42.666667-85.333333-42.666667-21.333333 42.666667-85.333333 42.666667-85.333333-42.666667-85.333334-42.666667-21.333333 42.666667-85.333333 42.666667-85.333333-42.666667-85.333333-42.666667-21.333333 42.666667-85.333334 42.666667v85.333333h853.333334v-85.333333z" fill="#2196F3" p-id="2478"></path><path d="M320 512H106.666667v64h277.333333c-64 0-64-64-64-64zM682.666667 490.666667s0 85.333333-64 85.333333h320v-85.333333H682.666667zM469.333333 153.749333h42.666667V576h-42.666667z" fill="#5D4037" p-id="2479"></path><path d="M277.333333 618.666667h42.666667v42.666666h-42.666667zM405.333333 618.666667h42.666667v42.666666h-42.666667zM533.333333 618.666667h42.666667v42.666666h-42.666667zM661.333333 618.666667h42.666667v42.666666h-42.666667z" fill="#3E2723" p-id="2480"></path><path d="M469.333333 133.226667v85.333333c83.541333-30.229333 161.792 21.333333 213.333334-85.333333-88.874667 60.501333-135.125333-26.666667-213.333334 0z" fill="#FF3D00" p-id="2481"></path><path d="M661.333333 256s64 64 42.666667 192h192s-85.333333-149.333333-234.666667-192zM618.666667 533.333333H365.034667c82.965333-128 0-277.333333 0-277.333333H618.666667s106.666667 149.333333 0 277.333333zM348.864 469.333333c22.613333-67.392 2.325333-136.448-11.242667-170.666666H170.666667s42.666667 85.333333 2.368 170.666666h175.829333z" fill="#90CAF9" p-id="2482"></path></svg>
  `
}
const ShipIcon = {
    template: `
    <a-icon :component="svgShip" />
  `,
    data() {
      return {
        svgShip,
      };
    },
  };
// header 组件
export default {
  name: 'BaseHeader',
  components: {
    ShipIcon
  }
}
</script>

<style lang="less" scoped>
.base-header{
  color: #fff;
  padding-top: 0.25rem;
  width: 100%;
  height: 5rem;
  background-image: url("../assets/sea-boats.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  .base-header__top{
    height: 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .base-header__logo{
    width: 100%;
    background: #fff;
    color: #333;
    border-radius: 0.5rem;
    .base-header__logo-logo{
      width: 0.48rem;
      vertical-align: middle;
    }
    .base-header__logo__desc{
      display: inline-block;
      font-size: 0.24rem;
      vertical-align: middle;
      padding-right: 0.2rem;
      span{
        margin-right: 0.1rem;
      }
    }
  }
  .base-header__nav{
    font-size: 0.22rem;
  }
}
</style>

