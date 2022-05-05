<template>
  <div class="footerUp container">
      <div class="container">
        <div class="col-left">
          <h2 class="title">DC Comics</h2>
          <ul class="listLink">
            <li v-for="(item, index) in dcComics" :key="index" >
              {{item.text}}
            </li>
           </ul>  
          <h2 class="title">SHOP</h2>
          <ul class="listLink">
            <li v-for="(item, index) in shop" :key="index" >
              {{item.text}}
            </li>
           </ul>  
        </div> <!-- /col-left-->
        <div class="col-center">
          <h2 class="title">DC</h2>
          <ul class="listLink">
            <li v-for="(item, index) in dc" :key="index" >
              {{item.text}}
            </li>
           </ul> 
        </div> <!-- /col-center-->
        <div class="col-right"> 
          <h2 class="title">SITES</h2>
          <ul class="listLink">
            <li v-for="(item, index) in sites" :key="index" >
              {{item.text}}
            </li>
           </ul>  
        </div> <!-- /col-right-->
      <img src="../assets/img/dc-logo-bg.png" alt="DC logo big"> 
      </div>
  </div>
 
</template>

<script>

export default {
  name:'FooterUp',
  data(){
    return{
      dcComics:[
        {  
          category: 'dc comics',
          text: 'Characters',
        },
        {  
          category: 'dc comics',
          text: 'Comics',
        },
        {  
          category: 'dc comics',
          text: 'Movies',
        },
        {  
          category: 'dc comics',
          text: 'TV',
        },
        {  
          category: 'dc comics',
          text: 'Games',
        },
        {  
          category: 'dc comics',
          text: 'Videos',
        },
        {  
          category: 'dc comics',
          text: 'News',
        }
        ],
        shop:[
        {  
          category: 'shop',
          text: 'Shop DC',
        },
        {  
          category: 'shop',
          text: 'Shop DC Collectibles',
        }
        ],
        dc:[
        {  
          category: 'dc',
          text: 'Term Of Use',
        },
        { 
          category: 'dc',
          text: 'Privacy policy (NEW)',
        },
        {  
          category: 'dc',
          text: 'Ad Choices',
        },
        {  
          category: 'dc',
          text: 'Advertising',
        },
        {  
          category: 'dc',
          text: 'Jobs',
        },
        {  
          category: 'dc',
          text: 'Subscriptions',
        },
        {  
          category: 'dc',
          text: 'Talent Workshops',
        },
        {  
          category: 'dc',
          text: 'CPSC Certificates',
        },
        {  
          category: 'dc',
          text: 'Ratings',
        },
        {  
          category: 'dc',
          text: 'Shop Help',
        },
        {  
          category: 'dc',
          text: 'Contact Us',
        }
        ],
        sites:[
        {  
          category: 'Sites',
          text: 'DC',
        },
        {  
          category: 'Sites',
          text: 'MAD Magazine',
        },
        {  
          category: 'Sites',
          text: 'DC Kids',
        },
        {  
          category: 'Sites',
          text: 'DC Universe',
        },
        {  
          category: 'Sites',
          text: 'DC Power Visa',
        },
      ]
    }
  }
     
}

</script>

<style lang="scss" scoped>
.footerUp{
  width: 100%;
  height: 370px;
  overflow: hidden;
}
.container{
  position: relative;
  display: flex;
  flex-flow: row wrap;
  justify-content: flex-start;
  align-content: center;
}
.title{
  text-transform: uppercase;
  color: #ffffff;
  margin: 20px;
}
ul{
  list-style-type: none;
  text-transform: uppercase;
  display: flex;
  flex-flow: column wrap;
  justify-content: flex-start;
  margin: 20px;
}
ul li{
  color: #959595;
  text-decoration: none;
  text-transform: capitalize;
  font-size: 12px;
  font-weight: 300;
  line-height: 1.5em;
}
.container img{
position: absolute;
top: -100px;
right: 0px;
height: 150%;
}

</style>