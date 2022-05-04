<template>
  <div id="app" class="container">
    <div><Navbar /></div>
    <div><Main /></div>
    <div><Navbar /></div>
    <div><Footer /></div>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
.container{
  border: 1px solid red;
  width: 100%;
  height: 100%;
}
</style>
