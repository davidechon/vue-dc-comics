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
}
.jumbotron{
  width: 100%;
  height: 370px;
  background-image: url('../assets/img/jumbotron.jpg');
  background-position: contain;
  background-size: 100%;
}
</style>