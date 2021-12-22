<template>
  <div class="about">
    <canvas
      width="100%"
      height="100%"
      class="flare canvas"
    ></canvas>
    <canvas
      width="100%"
      height="100%"
      class="snow canvas"
    ></canvas>
    <canvas
      width="100%"
      height="100%"
      class="flake canvas"
    ></canvas>
    <div style="text-align:center;">
    </div>
  </div>
</template>
<script>
import "../assets/js/jquery.let_it_snow"
export default {
  mounted () {
    this.$nextTick(() => {
      //闪光
      $("canvas.flare").let_it_snow({
        windPower: 0,
        speed: 0,
        color: "#392F52",
        size: 120,
        opacity: 0.00000001,
        count: 40,
        interaction: false
      });
      //雪花
      $("canvas.snow").let_it_snow({
        windPower: 3,
        speed: 1,
        count: 250,
        size: 0
      });
      //小碎片
      $("canvas.flake").let_it_snow({
        windPower: -3,
        speed: 1,
        count: 20,
        size: 10,
        image: require("../assets/images/white-snowflake.png")
      });
    })
  },
}
</script>
<style lang="scss" scoped>
@import url("../assets/css/style.css");
</style>