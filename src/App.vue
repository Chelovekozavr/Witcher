<template>
  <div id="app">
    <WitcherPromo />
    <WitcherLanding />
  </div>
</template>

<script>
  import WitcherLanding from './components/WitcherLanding.vue';
  import WitcherPromo from './components/WitcherPromo.vue';

  export default {
    name: 'App',
    components: {
      WitcherLanding,
      WitcherPromo
    }
  }
</script>

<style>
body {
  margin: 0;
}

h1, h2, h3, h4, h5, h6 {
  margin: 0;
}

#app {
  height: 100vh;
  width: 100vw;
  background-color: #000;

  background-image: url(./assets/images/bg.png);
    -moz-background-size: cover; /* Firefox 3.6+ */
    -webkit-background-size: cover; /* Safari 3.1+ и Chrome 4.0+ */
    -o-background-size: cover; /* Opera 9.6+ */
    background-size: cover;
    background-repeat: no-repeat;

    animation-name: fire-contrast;
    animation-duration: 5s;
    animation-iteration-count: infinite;
  
  overflow: hidden;
}

@keyframes fire-contrast {
    0%   {
      filter: blur(0);
      filter: contrast(1);
    }
    50% {
      filter: contrast(1.1);
    }

    100% {
      filter: contrast(1);
    }
}
</style>
