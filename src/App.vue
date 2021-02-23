<template>
  <div id="app">
    <ChargingMobile />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import ChargingMobile from "./components/ChargingMobile.vue";

@Component({
  components: {
    ChargingMobile
  }
})
export default class App extends Vue {}
</script>

<style>
#app {
  /* position: relative; */
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
}
</style>
