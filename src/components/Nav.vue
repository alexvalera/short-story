<template>
  <nav>
   <div>
    <p class = "nav__logo-type">shortstory</p>
   </div>
   <div v-show="allowLogin">
    <router-link to ="/login" class = "btn">Log In</router-link>
   </div>
  </nav>
</template>

<script>
export default {
  name: 'Nav',
  props: {
    allowLogin: Boolean
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang = "scss" scoped>
nav {
  display: flex;
  height: 50px; 
  padding: 0 1rem;
  div {
    align-self: center;
  }
  div:first-child {
    flex-grow: 1;
    text-align: left;
  }
  .nav__logo-type {
    font-weight: bold;
  }
  .btn {
    border: 1px solid #cecece;
    border-radius: 5px; 
    padding: 0.5rem;
    color: #777;
    text-decoration: none;
  }
}
</style>
