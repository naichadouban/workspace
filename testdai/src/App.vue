<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
      <helloMeta />
  </div>
</template>

<script>
    import helloMeta from "./components/hello-meta"
export default {
  name: "app",
  components: {
    helloMeta
  },
  beforeCreate () {
    console.log('registerWeb3 Action dispatched from casino-dapp.vue')
    this.$store.dispatch('registerWeb3')
  }
};
</script>

<style>
</style>
