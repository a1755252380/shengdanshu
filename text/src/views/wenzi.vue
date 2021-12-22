<template>
  <div class="wenzidiv">
    <h1
      aria-label="Test"
      class="scatter"
    >
      <span aria-hidden="true">M</span>
      <span aria-hidden="true">e</span>

      <span aria-hidden="true">r</span>
      <span aria-hidden="true">r</span>
      <span aria-hidden="true">y</span>
      <span aria-hidden="true">&nbsp;</span>
      <span aria-hidden="true">C</span>
      <span aria-hidden="true">h</span>
      <span aria-hidden="true">r</span>
      <span aria-hidden="true">i</span>
      <span aria-hidden="true">s</span>
      <span aria-hidden="true">t</span>
      <span aria-hidden="true">m</span>
      <span aria-hidden="true">a</span>
      <span aria-hidden="true">s</span>

    </h1>
  </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
.wenzidiv {
  width: 100%;
  position: absolute;
  top: 0;
  text-align: center;
}
.scatter {
  height: inherit;
}
.scatter span {
  position: relative;
  animation: scatter 2s infinite;
}

.scatter span:nth-child(2n) {
  animation-delay: 0.3s;
}

.scatter span:nth-child(3n) {
  animation-delay: 0.15s;
}

.scatter span:nth-child(5n) {
  animation-delay: 0.4s;
}

.scatter span:nth-child(7n) {
  animation-delay: 0.25s;
}

.scatter span:nth-child(9n) {
  animation-delay: 0.15s;
}

h1 {
  letter-spacing: 1px;
  //   margin: calc(50vh - 4rem) auto;
  text-align: center;
  font-family: "Archivo Black", "Archivo", sans-serif;
  font-weight: 400;
  text-transform: uppercase;
  font-size: 7rem;
  color: #ff9c55;
  text-shadow: -1px -1px #0d4e3b, -1px -0.75px #0d4e3b, -1px -0.5px #0d4e3b,
    -1px -0.25px #0d4e3b, -1px 0px #0d4e3b, 1px -1px #0d4e3b,
    1px -0.75px #0d4e3b, 1px -0.5px #0d4e3b, 1px -0.25px #0d4e3b,
    1px 0px #0d4e3b, 0px 1px #0d4e3b, -0.25px 1px #0d4e3b, -0.5px 1px #0d4e3b,
    -0.75px 1px #0d4e3b, -1px 1px #0d4e3b, 0 0.25px #0d4e3b, 0 0.5px #0d4e3b,
    0 0.75px #0d4e3b, -0.75px 0.75px #0d4e3b, -0.25px 0.25px #0d4e3b,
    1px 0.25px #0d4e3b, 1px 0.5px #0d4e3b, 1px 0.75px #0d4e3b, 1px 1px #0d4e3b,
    0px 6px #0d4e3b, -1px 6px #0d4e3b, -1px 5px #0d4e3b, -1px 5.75px #0d4e3b,
    -1px 5.5px #0d4e3b, -1px 5.25px #0d4e3b, -1px 4px #0d4e3b,
    -1px 4.75px #0d4e3b, -1px 4.5px #0d4e3b, -1px 4.25px #0d4e3b,
    -1px 3px #0d4e3b, -1px 3.75px #0d4e3b, -1px 3.5px #0d4e3b,
    -1px 3.25px #0d4e3b, -1px 2px #0d4e3b, -1px 2.75px #0d4e3b,
    -1px 2.5px #0d4e3b, -1px 2.25px #0d4e3b, -1px 1px #0d4e3b,
    -1px 1.75px #0d4e3b, -1px 1.5px #0d4e3b, -1px 1.25px #0d4e3b,
    1px 5px #0d4e3b, 1px 5.75px #0d4e3b, 1px 5.5px #0d4e3b, 1px 5.25px #0d4e3b,
    1px 4px #0d4e3b, 1px 4.75px #0d4e3b, 1px 4.5px #0d4e3b, 1px 4.25px #0d4e3b,
    1px 3px #0d4e3b, 1px 3.75px #0d4e3b, 1px 3.5px #0d4e3b, 1px 3.25px #0d4e3b,
    1px 2px #0d4e3b, 1px 2.75px #0d4e3b, 1px 2.5px #0d4e3b, 1px 2.25px #0d4e3b,
    1px 1px #0d4e3b, 1px 1.75px #0d4e3b, 1px 1.5px #0d4e3b, 1px 1.25px #0d4e3b;
}

h1 span:nth-child(2n) {
  color: #f47aff;
}

h1 span:nth-child(3n) {
  color: #ffd913;
}

h1 span:nth-child(5n) {
  color: #555bff;
}

h1 span:nth-child(7n),
h1 span:nth-child(12n) {
  color: #ff5555;
}

@keyframes scatter {
  0% {
    top: 0;
  }
  50% {
    top: -10px;
  }
  100% {
    top: 0;
  }
}

@media screen and (max-width: 760px) {
  h1 {
    font-size: 2rem;
  }
  .wenzidiv {
    top: 10%;
  }
}
</style>