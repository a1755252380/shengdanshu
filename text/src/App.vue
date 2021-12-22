<template>
  <div id="app">
    <about class="back"></about>
    <router-view />
    <wenzi class="wenzi"></wenzi>
  </div>
</template>
<script>
import about from './views/About.vue'
import wenzi from "./views/wenzi.vue"

export default {
  components: {
    about,
    wenzi
  }
}
</script>
<style lang="scss">
@import url("./assets/html.css");
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  // background: #000;
}
.back {
  position: fixed;
  z-index: -1;
}
</style>
