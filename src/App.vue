<template>
  <div id="app">
    <div><Header /></div>
    <!-- <div><Navbar /></div> -->
    <div><Main /></div>
    <div><Footer /></div>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>
<style lang="sass" scoped>
@import './assets/css/general.css'
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,300;0,400;0,600;0,900;1,100;1,300;1,400;1,600;1,900&display=swap')
</style>
