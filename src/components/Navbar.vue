<template>
 <nav class="container clearfix">
  <div class="logo">
      <a href="#" class="logo">
          <img src="../assets/img/dc-logo.png" alt="logo">
      </a>
  </div>
  <ul>
      <li v-for="(item, index) in links" :key="index" :class="{'selected' : item.active}"><a href="#">{{item.text}}</a></li>
      
  </ul>   
</nav>
</template>

<script>
export default {
  name: 'Navbar',
  data(){
    return{
    links:[
    {  
      text: 'CHARACTER',
      link: '',
      active: false,
    },
    {
      text: 'COMICS',
      link: '',
      active: false,
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
.clearfix:after {
    content: "";
    display: table;
    clear: both;
}
.container{
    width: 80%;
    margin: 0 auto;
}
nav{
    width: 100%;
    height: 120px;
    line-height: 120px;
    // background-color: rgba(49,97,224,255);
    // position: fixed;
    // z-index: 1;
}
nav .logo, nav ul{
    display: flex;
    flex-flow: row nowrap;
    // justify-content: space-around;
    
}
nav .logo img{
  border: 1px solid blue;
  display: flex;
  flex-flow: row nowrap;
  justify-items: flex-start;
    align-content: center;
}
nav ul {
  border: 1px solid blue;
    list-style-type: none;
    width: 80%;
    text-align: center;
    font-size: 14px;
}
nav ul li {
    display: inline-block;
}
nav ul li a{
    text-decoration: none;
    margin: 0 20px;
    color: #000000;
}
nav ul li a:hover {
    border-bottom: 1px solid blue;
}
</style>