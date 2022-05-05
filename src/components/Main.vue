<template>
   <main class="container-fluid">
  <div class="main">
    <div> <Jumbotron /> </div>
    <div> <Cards /> </div>
    <div> <RowIconsBuy /> </div>
   
    
  </div>
  </main>
</template>

<script>

import Jumbotron from '../components/Jumbotron.vue';
import Cards from '../components/Cards.vue';
import RowIconsBuy from '../components/RowIconsBuy.vue';

export default {
  name:'Main',
  components: {
      Jumbotron,
      Cards,
      RowIconsBuy,
    
  }
     
}
</script>

<style lang="scss">
.main{
  width: 100%;
  color: #ffffff;
}
</style>