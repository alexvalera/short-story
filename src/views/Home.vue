<template>
  <div class="home">
    <Nav v-bind:allowLogin="true"/>
    <Intro/>
  </div>
</template>

<script>
// @ is an alias to /src
//import HelloWorld from '@/components/HelloWorld.vue'
import Nav from '@/components/Nav.vue'
import Intro from '@/components/Intro.vue'
export default {
  name: 'home',
  components: {
    Nav,
    Intro
  }
}
</script>
