<template>
  <section>
    <div>
      <h1>No more BS. Let everyone know what's up.</h1>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Intro',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang = "scss" scoped>
section {
  display: flex; 
  align-items: center;
  justify-content: center;
  height: calc(100vh - 50px);
}
</style>
