<template>
  <div class="container-fluid rowIconsBuy">
    <div class="iconsBuy">
      <ul>
          <li v-for="(icon, index) in icons" :key="index">
            <img :src="icon.img" :alt="icon.text">
            <span :class="iconText">{{icon.text}}</span>
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
          img: '../assets/img/buy-comics-digital-comics.png',
        },
        {
          text: 'dc merchandise',
          img: '../assets/img/buy-comics-merchandaise.png',
        },
        {
          text: 'subscription',
          img: '../assets/img/buy-comics-subscriptions.png',
        },
        {
          text: 'comin shop locator',
          img: '../assets/img/buy-comics-shop-locator.png',
        },
        {
          text: 'dc power visa',
          img: '../assets/img/buy-dc-power-visa.svg',
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
  // background-color: #ffffff;
}
.iconImg{
  color:lime;
}
.iconText{
  color:red;
}
</style>