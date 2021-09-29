<template>
  <div>
    <b-navbar type="dark" variant="dark">
      <b-navbar-nav>
        <b-nav-item href="#">{{msg}}</b-nav-item>
        <b-nav-item-dropdown v-model="msg" text="Coin" right>
          <b-dropdown-item href="#" v-for="coin in coins" v-bind:key="coin">{{coin}}</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-navbar>
    <div>
      <h2> {{msg}} </h2>
    </div> 
  </div>   
</template>

<script>
export default {
  name: 'NavBar',
  data(){
    return{
      coins: ['BTC',
      'ETH',
      'AXS',
      'CASH'
      ],
      msg: "Bitcoin"
    }
  },
  methods:{ 
    
  }
}
</script>

<style scoped>
  h2{
    margin-left: auto;
    margin-right: auto;
    width: 6em
}
</style>
