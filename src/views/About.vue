<template>
  <div class="about">
    <h1>This is an about page</h1>
    <a-carousel effect="fade">
      <div v-for="(item,idx) in imgList" :key="idx" :style="{background: 'url('+item.url+')',color: 'red',width: '100%', height: '100%', backgroundOrigin: 'content-box',backgroundRepeat: 'no-repeat',backgroundSize: 'cover',backgroundPosition: 'center'}" class="bg-img__wrapper">
        <span>{{item.desc}}</span>
      </div>
    </a-carousel>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        imgList: [
          {
            url: require("../assets/seaAlone.jpg"),
            desc: "https://magdeleine.co/browse/"
          },
          {
            url: require("../assets/alone.jpg"),
            desc: "https://magdeleine.co/browse/"
          },
          {
            url: require("../assets/sea-boats.jpg"),
            desc: "https://magdeleine.co/browse/"
          }
        ]
      }
    }
  };
</script>
<style scoped>
  /* For demo */
  .ant-carousel >>> .slick-slide {
    text-align: center;
    height: 4.5rem;
    line-height: 4.5rem;
    background: #364d79;
    overflow: hidden;
  }

  .ant-carousel >>> .slick-slide h3 {
    color: #fff;
  }
</style>