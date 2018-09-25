<template>
  <div class="login">
    <Nav v-bind:allowLogin="false"/>
    <Login/>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import Nav from '@/components/Nav.vue'
import Login from '@/components/Login.vue'
export default {
  name: 'home',
  components: {
    Nav, 
    Login
  }
}
</script>
