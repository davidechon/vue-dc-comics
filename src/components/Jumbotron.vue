<template>
  <div class="container-fluid">
    <div class="jumbotron">
    </div>
  </div>
</template>

<script>
export default {
  name:'Jumbotron',
}
</script>

<style lang="scss" scoped>
.container-fluid{
  width: 100%;
  border: 4px solid pink;
}
.jumbotron{
  width: 100%;
  height: 280px;
  background-image: url('../assets/img/jumbotron.jpg');
  background-size: cover;
  
}
</style>