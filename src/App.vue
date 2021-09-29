<template>
  <div id="app">
    <nav-bar/>
    <card/>
   
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import Card from './components/Card.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    Card
  }
}
</script>

<style>

</style>
