<template>
  <div class="container-fluid rowIconsBuy">
      <div class="iconsBuy">
      <ul>
          <li v-for="(icon, index) in icons" :key="index">
            <img class="iconImg" :src="icon.src" :alt="icon.text">
            <span :class="icon.text">{{icon.text}}</span>
          </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RowIconsBuy',
  data(){
    return{
      icons:[
        {  
          text: 'digital comics',
          // img: '../img/buy-comics-digital-comics.png',
          src: './img/buy-comics-digital-comics.png',
          
        },
        {
          text: 'dc merchandise',
          src: './img/buy-comics-merchandise.png',
        },
        {
          text: 'subscription',
          src: './img/buy-comics-subscriptions.png',
        },
        {
          text: 'comin shop locator',
          src: './img/buy-comics-shop-locator.png',
        },
        {
          text: 'dc power visa',
          src: './img/buy-dc-power-visa.svg',
        }
      ]
    }
  }
 
}
</script>

<style lang="scss" scoped>
.rowIconsBuy{
  width: 100%;
  background: #0282f9;
  height: 150px;
  display: flex;
  justify-content: center;
  align-items: center;
  
}
.iconsBuy ul{
  display: inline-flex;
}
.iconsBuy ul li{
  list-style-type: none;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  align-items: center;
  color: #ffffff;
}
.iconsBuy ul li .iconImg{
  width: 60px;
  height: auto;
  padding: 10px;
  
}
// .iconText{
//   color:red;
// }
</style>