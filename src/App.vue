<template>
  <div id="app">
    <nav-bar/>
    <Coin msg="Bitcoin"/>
    <card/> 
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import Card from './components/Card.vue'
import Coin from './components/Coin.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    Coin,
    Card,
    
  }
}
</script>

<style>

</style>
