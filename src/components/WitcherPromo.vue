<template>
  <div class="promo">
    <h2 class="promo__text-title">300%</h2>
    <h3 class="promo__text">Welcome bonus</h3>
    <div class="promo__code-container">
      <h1 class="propmo__main-title">Witcher</h1>
    </div>
    <div>
      <span class="promo__copy-code">Copy code</span>
    </div>
    <button class="promo__button"></button>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>
  .promo {
    font-family: Cambria;
    position: absolute;
    top: 200px;
    right: 10vw;
  }

  .promo__text-title {
    font-family: Cambria;
    font-size: 208.55px;
    color: #fff;
  }

  .promo__text {
    font-family: Cambria;
    font-size: 67.58px;
    color: #fff;

    text-transform: uppercase;
  }

  .promo__code-container {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 20px;
    height: 80px;
    width: 270px;
    border-radius: 40px;
    border: 1px solid grey;

    text-transform: uppercase;
  }

  .propmo__main-title {
    font-family: Arial;
    font-size: 40px;
    color: #f73427;
  }
</style>