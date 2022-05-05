<template>
  <footer class="footer container-fluid">
    <div class="footerUp"><FooterUp /></div>
    <div class="footerDown"><FooterDown /></div>
  </footer>
</template>

<script>

import FooterUp from '../components/FooterUp.vue';
import FooterDown from '../components/FooterDown.vue';

export default {
  name:'Footer',
  components: {
      FooterUp,
      FooterDown,
  }
     
}

</script>

<style lang="scss" scoped>
.footer{
  width: 100%;
  height: 370px;
  background-image: url('../assets/img/footer-bg.jpg');
  background-position: contain;
  background-size: 100%;
}
</style>