<template>
  <Hero header="NFT"/>
</template>

<script>
import Hero from './components/Hero.vue'

export default {
  name: 'App',
  components: {
    Hero
  }
}
</script>

<style>
* {
    margin: 0;
    padding: 0;
}
body {
    width: 100%;
    height: 100%;
    overflow-x: hidden;
    overflow-y: hidden;
    background-color:  #f5f5f5;
    font-family: 'PT Serif', serif;
}
#app {
  text-align: center;
}
</style>
