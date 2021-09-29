<template>
  <div>
    <div>
      <b-card-group deck>
        <b-card  bg-variant="dark" text-variant="white"  class="text-center" v-for="(item, index) in coin.ticker" v-bind:key="(item, index)">
          <b-card-header>{{index}}</b-card-header>
          <b-card-text>{{item}}</b-card-text>
        </b-card>      
      </b-card-group>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  data(){
    return{
      coin: []
    }
  },
  methods: {
    fetchItem() {
      fetch('https://www.mercadobitcoin.net/api/BTC/ticker/')
      .then(res => res.json())
      .then(data => this.coin = data)

    }
  },
  created() {
    this.fetchItem()
  }
}
</script>
<style>
div .card{
  margin: 10px;
  max-width: 20rem;
  cursor: pointer;
}
</style>