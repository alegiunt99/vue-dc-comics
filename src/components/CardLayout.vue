<template>
  <div class="card">
      <img :src="card.thumb">
      <h2>{{card.series}}</h2>

  </div>
</template>

<script>
export default {
    name: 'CardLay',

    props:{
        card: Object
    }

}
</script>

<style lang="scss" scoped>

</style>