<template>
  <header class="container">
        <Navbar />
    </header>
</template>

<script>
import Navbar from '../components/Navbar.vue';

export default {
 name: 'Header',
 components: {
    Navbar,
    
  }
}
</script>

<style lang="scss" scoped>

header{
    width: 100%;
    height: 120px;
    line-height: 120px;
    // background-color: rgba(49,97,224,255);
    // position: fixed;
    // z-index: 1;
}

</style>