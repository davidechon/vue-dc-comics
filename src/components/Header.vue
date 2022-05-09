<template>
  <header class="container-fluid">
    <img
      src="../assets/img/dc-logo.png"
      alt="logo"
      class="logo"
    />
    <nav>
      <ul>
          <li v-for="(item, index) in links" :key="index" :class="{'selected' : item.active}">{{item.text}}</li>
      </ul>  
    </nav>
  </header>
</template>

<script>


export default {
 name: "Header",
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
@import "@/assets/css/general.scss";

header {
  height: 100px;
  margin-bottom: 30px;
  position: relative;

  .logo {
    position: absolute;
    top: 10px;
    left: 20px;
    width: 80px;
    height: 80px;
    line-height: 70px;
  }
  .navbar{
    height: 100px;
    display: flex;
    flex-flow: row nowrap;
    border: 1px solid blue;
    // position: relative;
    ul {
      // position: absolute;
      // top: 0;
      // right: 0;
      list-style-type: none;
      max-width: 100%;;
      height: 80px;
      text-align: center;
      font-size: 14px;
      text-transform: uppercase;
      font-weight: 600;
      display: flex;
      flex-flow: row nowrap;
      justify-content: flex-end;
    }
    ul li{
      text-decoration: none;
      margin: 0 5px;
    }
    .selected{
      border-bottom: 6px solid #0282f9;
    } 
  }
}

</style>