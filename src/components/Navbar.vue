<template>
 <nav class="container">
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="logo">
      <ul>
          <li v-for="(item, index) in links" :key="index" :class="{'selected' : item.active}">{{item.text}}</li>
      </ul>  
    </div> 
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
  data(){
    return{
    links:[
    {  
      text: 'character',
      link: '',
      active: false,
    },
    {
      text: 'COMICS',
      link: '',
      active: true,
    },
    {
      text: 'MOVIES',
      link: '',
      active: false,
    },
    {
      text: 'TV',
      link: '',
      active: false,
    },
    {
      text: 'GAMES',
      link: '',
      active: false,
    },
    {
      text: 'COLLECTIBLES',
      link: '',
      active: false,
    },
    {
      text: 'VIDEOS',
      link: '',
      active: false,
    },
    {
      text: 'FANS',
      link: '',
      active: false,
    },
    {
      text: 'NEWS',
      link: '',
      active: false,
    },
    {
      text: 'SHOP',
      link: '',
      active: false,
    }
    ]
    }
  }
 
}
</script>

<style lang="scss" scoped>

nav{
  height: 100px;
  display: flex;
  flex-flow: row nowrap;
  position: relative;
}
nav .logo img{
  position: absolute;
  width: 70px;
  top: 10px;
  left: 10px;
  line-height: 100px;
  vertical-align: middle;
}
nav ul {
  position: absolute;
  top: 0;
  right: 0;
  list-style-type: none;
  height: 100px;
  text-align: center;
  font-size: 14px;
  text-transform: uppercase;
  font-weight: 600;
  display: flex;
  flex-flow: row nowrap;
  justify-content: flex-end;
}
nav ul li{
  text-decoration: none;
  margin: 0 10px;
}
.selected{
  border-bottom: 6px solid #0282f9;
} 

</style>