<template>
  <div style="height: 100%">
    <Base />
    <!-- <div class="title"></div> -->

    <img src="../assets/2_title.png" alt="" class="title" />
    <img :src="imgUrl[0]" alt="" class="battery" />
    <p class="num">98%</p>
  </div>
</template>

<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
import Base from "./Base.vue";

@Component({
  components: {
    Base
  }
})
export default class Slide1 extends Vue {
  g1 = require("../assets/2_g1.png");
  imgUrl = [
    require("../assets/2_g1.png"),
    require("../assets/2_g2.png"),
    require("../assets/2_g3.png"),
    require("../assets/2_g4.png")
  ];
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
img {
  position: absolute;
  margin: 0 auto;
  left: 0;
  right: 0;
}
.title {
  width: 70%;
  top: 13%;
}
.battery {
  width: 55%;
  /* top: 240px; */
  bottom: 0;
}
@font-face {
  font-family: "cc";
  src: url("../assets/YouSheBiaoTiHei-2.ttf");
}
p {
  position: absolute;
  top: 20%;
  left: 0;
  right: 0;
  margin: 0 auto;
  font-size: 68px;
  font-family: cc;
  color: #f3e228;
}
</style>
