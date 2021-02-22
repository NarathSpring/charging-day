<template>
  <swiper ref="mySwiper" :options="swiperOptions" class="swiper-container">
    <swiper-slide class="slide1">1111111111111111</swiper-slide>
    <swiper-slide class="slide2">22222222222222222</swiper-slide>
    <swiper-slide class="slide3">33333333333333333</swiper-slide>
  </swiper>
</template>

<script lang="ts">
import { Vue } from "vue-property-decorator";
import { SwiperOptions } from "swiper";

export default class ChargingMobile extends Vue {
  swiperOptions: SwiperOptions = {
    effect: "fade",
    direction: "vertical",
    speed: 300,
    freeMode: false
  };
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
swiper-slide {
  height: 300px;
}
.slide1 {
  background: blue;
}
.slide2 {
  background: red;
}
.slide3 {
  background: yellow;
}
.swiper-container {
  width: 100%;
  height: 100%;
}
</style>
