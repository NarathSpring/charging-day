<template>
  <div class="base">
    <img src="../assets/top.png" alt="" class="top" />
  </div>
</template>

<script lang="ts">
import { Vue } from "vue-property-decorator";

export default class Base extends Vue {}
</script>

<style scoped>
.base {
  position: relative;
  background: url("../assets/background.png");
  background-size: cover;
  height: 100%;
}
.top {
  width: 50%;
  position: absolute;
  top: 30px;
  left: 0;
  right: 0;
  margin: 0 auto;
}
</style>
