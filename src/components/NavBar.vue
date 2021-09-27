<template>
  <div>
    <b-navbar type="dark" variant="dark">
      <b-navbar-nav>
        <b-nav-item href="#">Home</b-nav-item>

        <!-- Navbar dropdowns -->
        <b-nav-item-dropdown text="Coin" right>
          <b-dropdown-item href="#">BTC</b-dropdown-item>
          <b-dropdown-item href="#">ETH</b-dropdown-item>
          <b-dropdown-item href="#">CASH</b-dropdown-item>
          <b-dropdown-item href="#">AXS</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    msg: String
  }
}
</script>

<style scoped>

</style>
