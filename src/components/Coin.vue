<template>
  <div>
  <h2> {{msg}} </h2>
  </div>
</template>

<script>
export default {
  name: 'Coin',
  props: {
    msg: String
  }
}
</script>
<style>
h2{
    margin-left: auto;
    margin-right: auto;
    width: 6em
}
</style>
