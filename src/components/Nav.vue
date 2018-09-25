<template>
  <nav>
    hello
  </nav>
</template>

<script>
export default {
  name: 'Nav',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang = "scss" scoped>
nav {
  height: 50px; 
  background-color: #1abc9a;
}
</style>
