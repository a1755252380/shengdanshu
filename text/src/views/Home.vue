<template>
  <div class="tree">
    <canvas
      id="c"
      :height="height"
      :width="width"
    ></canvas>
    <div class="treediv">&nbsp;</div>

  </div>
</template>

<script>
import "../assets/tree"
export default {
  name: 'Home',
  components: {
  },
  data () {
    return {
      width: 1440,
      height: 900
    }
  },
  mounted () {
  },
}
</script>
<style lang="scss" scoped>
.treediv {
  width: 60px;
  height: 90px;
  background-color: #5a3200;
  background-image: linear-gradient(
    90deg,
    #5a3200 0%,
    #a96107 31%,
    #b36405 56%,
    #a96006 78%,
    #5a3200 99%
  );

  position: absolute;
  box-shadow: 0px 0px 5px 5px #363636;

  top: 500px;
  left: 190px;

  z-index: -1;
}
@media (min-width: 0px) and (max-width: 768px) {
  .tree {
    position: absolute;
    bottom: -80px !important;
    left: -15px !important;
  }
}
.tree {
  position: absolute;
  bottom: -80px;
  left: 40%;
}
#c {
  z-index: 999;
}
div {
  margin: 0;
  padding: 0;
  border: 0;
}

.nav {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 27px;
  background-color: white;
  color: black;
  text-align: center;
  line-height: 25px;
}

a {
  color: black;
  text-decoration: none;
  border-bottom: 1px dashed black;
}

a:hover {
  border-bottom: 1px solid red;
}

.previous {
  float: left;
  margin-left: 10px;
}

.next {
  float: right;
  margin-right: 10px;
}

.green {
  color: green;
}

.red {
  color: red;
}

textarea {
  width: 100%;
  height: 100%;
  border: 0;
  padding: 0;
  margin: 0;
  padding-bottom: 20px;
}

.block-outer {
  float: left;
  width: 22%;
  height: 100%;
  padding: 5px;
  border-left: 1px solid black;
  margin: 30px 3px 3px 3px;
}

.block-inner {
  height: 68%;
}

.one {
  border: 0;
}
</style>
