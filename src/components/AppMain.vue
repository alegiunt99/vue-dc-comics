<template>
  <main class="main-page">
    <!-- Jumbotron -->
    <div class="jumbotron">
    </div>

    <!-- Parte centrale con le card de i fumetti -->
    <div class="container">
      <Card v-for="(item, index) in ComicsPhotos" :key="index" :card="item"/>
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
}

</style>
