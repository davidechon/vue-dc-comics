<template>
   <main class="container">
  <div class="main">
    <RowContent />
  </div>
  </main>
</template>

<script>

import RowContent from '../components/RowContent.vue';
export default {
  name:'Main',
  components: {
      RowContent,
    
  }
     
}
</script>

<style lang="scss" scoped>
.main{
  // border: 1px solid red;
  width: 100%;
  height: 500px;
  color: #ffffff;
}
</style>