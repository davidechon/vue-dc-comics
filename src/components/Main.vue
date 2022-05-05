<template>
   <main class="container">
  <div class="main">
    <!-- <div> <RowContent /> </div> -->
    <div> <Cards /> </div>
    <div> <RowIconsBuy /> </div>
   
    
  </div>
  </main>
</template>

<script>

// import RowContent from '../components/RowContent.vue';
import Cards from '../components/Cards.vue';
import RowIconsBuy from '../components/RowIconsBuy.vue';

export default {
  name:'Main',
  components: {
      // RowContent,
      Cards,
      RowIconsBuy,
    
  }
     
}
</script>

<style lang="scss" scoped>
.main{
  border: 1px solid red;
  width: 100%;
  color: #ffffff;
}
</style>