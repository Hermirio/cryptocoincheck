<template>
  <div>
    <div class="teste"  >
      <b-card-group deck>
        <b-card bg-variant="dark" text-variant="white" header="Dark" class="text-center">
          <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</b-card-text>
        </b-card>
      </b-card-group>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    msg: String
  }
}
</script>
<style>
.teste{
  margin: auto;
  transform: translateY(-5px);
  cursor: pointer;
}
</style>
