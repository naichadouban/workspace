<template>
    <h1>hello Metamask</h1>
    <p>Metamask: {{ web3.isInjected }}</p>
    <p>Network: {{ web3.networkId }}</p>
    <p>Account: {{ web3.coinbase }}</p>
    <p>Balance: {{ web3.balance }}</p>
</template>

<script>
  export default {
    name: "hello-meta",
    computed:{
      web3(){
        return this.$store.state.web3
      }
    }
  }
</script>

<style scoped>

</style>