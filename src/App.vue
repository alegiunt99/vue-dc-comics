<template>
  <div id="app">
    <HeaderApp />
    <MainApp :ComicsPhotos="ComicsPhotos"/>
    <FooterApp />
  </div>
</template>

<script>
import HeaderApp from './components/AppHeader.vue';
import MainApp from './components/AppMain.vue';
import FooterApp from './components/AppFooter.vue';

// data
import ComicsPhotos from '@/assets/data/dc-comics.json'
console.log(ComicsPhotos)
export default {
  name: 'App',

  data(){

    return { ComicsPhotos }
  },

  components: {
    HeaderApp,
    MainApp,
    FooterApp
  }
}
</script>

<style lang="scss">
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

.container{
  width: 80%;
  margin: 0 auto;
}
</style>
