<template>
  <main class="main-page">
    <!-- Jumbotron -->
    <div class="jumbotron">
    </div>

    <!-- Parte centrale con le card de i fumetti -->
    <div class="central-page">
      <div class="container">
        <Card v-for="(item, index) in ComicsPhotos" :key="index" :card="item"/>
      </div>
      <div id="load-more">
        <button>
          LOAD MORE
        </button>
      </div>
    </div>
    
  </main>
</template>

<script>

import Card from '@/components/CardLayout.vue'

export default {
  name: 'MainApp',

  props: {
    ComicsPhotos: Array,
  },

  components:{
    Card
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.main-page{
  .jumbotron{
    height: 280px;
    background-image: url('@/assets/jumbotron.jpg');
    background-size: cover;
  }
  .central-page{
    background-color: rgb(46, 46, 46);
    padding: 50px 0px;
    .container{
    display: flex;
    flex-wrap: wrap;
    column-gap: 5px;
    row-gap: 20px;
  }

  #load-more{
    text-align: center;
    button{
      background-color: #0282f9;
      font-size: 14px;
      padding: 10px;
      color: white;
      border: none;
      &:hover{
        background-color: rgb(104, 104, 104);
        cursor: pointer;
      }
    }
  }
  }
  
  
}

</style>
