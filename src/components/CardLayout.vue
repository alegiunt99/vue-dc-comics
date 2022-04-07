<template>
  <div class="card">
      <img :src="card.thumb">
      <h5>{{card.series}}</h5>
      <p>{{card.price}}</p>
      <span>{{card.type}}</span>

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
    .card{
        width: 16%;

        h5{
            color: white;
            font-size: 16px;
            margin: 5px 0px;
        }

        img{
            width: 85%;
        }

        p,
        span{
            font-size: 15px;
            color: gray;
        }
    }
</style>