<template>
  <div class="footerUp container">
      <div class="container  menuFooter">
        <ul>
          <li v-for="(item, index) in menuItems" :key="index" >
            {{item.text}}
          </li>
      </ul>   
      </div>
  </div>
 
</template>

<script>

export default {
  name:'FooterUp',
  data(){
    return{
      menuItems:[
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
        },
        {  
          category: 'shop',
          text: 'Shop DC',
        },
        {  
          category: 'shop',
          text: 'Shop DC Collectibles',
        },
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
        },
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
  border: 2px solid violet;
  width: 100%;
  height: 370px;
}
.menuFooter ul{
  list-style-type: none;
  text-transform: uppercase;
  display: flex;
  flex-flow: column wrap;
  justify-content: flex-start;
}
.menuFooter ul li{
  color: #ffffff;
  text-decoration: none;
  text-transform: uppercase;
  
}
</style>