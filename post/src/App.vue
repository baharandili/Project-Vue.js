<template>
  <!-- <img alt="Vue logo" src="./assets/in-love.png"> -->
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Hai Cantik, Pencet Tombol Dibawah Yaaa"/> -->
  <HelloWorld msg="Vue test"/>
  <!-- <h1>AKU GANTENK</h1> -->
  <!-- <PAGES /> -->
  <!-- <pages_One /> -->
  <!-- <input_box /> -->
  <!-- <ifElse /> -->
  <!-- <for_loops /> -->
  <Kampus/>
</template>
<script>
import HelloWorld from './components/HelloWorld.vue'
import Kampus from './components/kampus.vue';
// import PAGES from './components/NewTest.vue'
// import pages_One from './components/pages.vue'
// import input_box from './components/inputbox.vue'
// import ifElse from './components/ifelse.vue'
// import for_loops from './components/loops.vue'
export default {
  name: 'App',
  components: {
    HelloWorld,
    Kampus
}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
