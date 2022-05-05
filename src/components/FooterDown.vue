<template>
  <div class="footerDown container-fluid">
    <div class="container">
      <div class="btn-signUp">Sign-up now&#x21;</div>
      <div class="followUs">
        <h2>Follow Us</h2>
        <ul>
          <li><img src="../assets/img/footer-facebook.png" alt="Facebook"></li>
          <li><img src="../assets/img/footer-twitter.png" alt="twitter"></li>
          <li><img src="../assets/img/footer-youtube.png" alt="youtube"></li>
          <li><img src="../assets/img/footer-pinterest.png" alt="pinterest"></li>
          <li><img src="../assets/img/footer-periscope.png" alt="periscope"></li>
        </ul>
      </div>
    </div>
    
  </div>
 
</template>

<script>

export default {
  name:'FooterDown',
  
     
}

</script>

<style lang="scss" scoped>
.container-fluid{
  width:100%;
}
.container{
  width: 80%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-items: center;
}
.footerDown{
  background-color: #303030;
  height: 100px;
  margin: 0 auto;
  padding: 10px;
}
.btn-signUp{
  color: #ffffff;
  border: 3px solid #0282f9;
  padding: 10px;
  text-transform: uppercase;
  text-align: center;
  width: 150px;
}
.btn-signUp:hover{
  color: #0282f9;
  border: 3px solid #ffffff;
}
.followUs{
  color: #0282f9;
  position: relative;
  width: 50%;
  display: flex;
  flex-flow: row nowrap;
  justify-content: flex-end;
  align-items: center;
}
.followUs h2{
  color: #0282f9;
  text-transform: uppercase;
  margin-right: 20px;
  font-size: 16px;
}
.followUs ul li{
  list-style: none;
  display: inline-block;
}
.followUs img{
  width: 30px;
  height: auto;
  margin: 10px;
}
.followUs img:hover{
  background-color: #fff;
  border-radius: 50%;
  cursor: pointer;
}
</style>