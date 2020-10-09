<template>
  <div class="main-container">
    <img
      src="../assets/images/witcher.png"
      alt="Witcher"
      class="witcher"
    >
    <img
      src="../assets/images/sparks_back_blured.png"
      alt="Witcher"
      class="sparks-back"
    >

    <img
      src="../assets/images/sparks_back.png"
      alt="Witcher"
      class="sparks-back2"
    >
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

@font-face {
 font-family: 'Cambria';
  src: url('../assets/fonts/cambriab.ttf');
}

.test {
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
  font-size: 100px;
}

h1 {
  margin: 0;
}

.main-container {

}

.witcher {
  position: absolute;
  left: 5px;
  top: -40px;
  transform: scale(0.9);
  z-index: 1;
}

.sparks-back {
  position: absolute;
  left: 100px;
  top: 20;
  transform: rotate(180deg);

  animation-name: sparks-top;
  animation-duration: 30s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;

  z-index: 2;
}

.sparks-back2 {
  position: absolute;
  left: 5px;
  top: -40px;

  animation-name: sparks-top2;
  animation-duration: 25s;
  animation-iteration-count: infinite;
  animation-timing-function: ease;
}

@keyframes sparks-top {
  0%   {
    top: -40px;
    filter: blur(5px);
    transform: scale(0.8);
  }
  100% {
    top: -400px;
    filter: blur(5px);
    transform: scale(1);
  }
}

@keyframes sparks-top2 {
  0% {
    transform: scale(0.8);
  }
  100% {
    transform: scale(1);
  }
}

</style>
