<template>
  <div style="height: 100%">
    <Base />
    <!-- <div class="title"></div> -->

    <img src="../assets/1_title.png" alt="" class="title" />
    <img src="../assets/1_battery.png" alt="" class="battery" />
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
export default class Slide1 extends Vue {}
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
  top: 120px;
}
.battery {
  width: 40%;
  top: 240px;
}
</style>
