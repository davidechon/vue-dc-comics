<template>
  <div class="cards-container">
    <div class="card-group">
      <ul>
          <li v-for="(card, index) in cards" :key="index">
            <img class="card" :src="cards.thumb" :alt="cards.series">
            <span :class="cards.series">{{cards.series}}</span>
          </li>
      </ul>
    </div> 
  </div>
</template>

<script>

export default {
  name: 'Cards',
  data() {
    return{
      cards:[
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
      ]
    }
  },
}
</script>



<style lang="scss" scope>
.cards-container{
  border: 4px solid yellow;
  width: 100%;
  height: 100px;
  display: flex;
  align-items: center;
  
}
.cards-group{
  border: 4px solid yellow;
  width: 100%;
  height: 500px;
}
.card{
  border: 4px solid yellow;
  width: 100%;
  height: 500px;
}
</style>