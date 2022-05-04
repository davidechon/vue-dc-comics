<template>
  <header class="container-fluid">
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
    line-height: 100px;
    background-color: #fff;
    margin-bottom: 0;
}

</style>