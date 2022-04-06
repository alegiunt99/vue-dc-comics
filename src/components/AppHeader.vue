<template>
  <header class="header-page">
    <!-- creo la classe container che centra il contenuto-->
    <div class="container">

      <!-- il div del logo -->
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="Logo DC-Comics">
      </div>

      <!-- il div della barra di navigazione -->
      <div class="nav-bar">
        <div class="nav-link"><a href="#"></a>CHARACTERS</div>
        <div class="nav-link"><a href="#"></a>COMICS</div>
        <div class="nav-link"><a href="#"></a>MOVIES</div>
        <div class="nav-link"><a href="#"></a>TV</div>
        <div class="nav-link"><a href="#"></a>GAMES</div>
        <div class="nav-link"><a href="#"></a>COLLECTIBLES</div>
        <div class="nav-link"><a href="#"></a>VIDEOS</div>
        <div class="nav-link"><a href="#"></a>FANS</div>
        <div class="nav-link"><a href="#"></a>NEWS</div>
        <div class="nav-link"><a href="#"></a>SHOP</div>
      </div>

    </div>
    
  </header>
</template>

<script>
export default {
  name: 'HeaderApp',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 0;
    .logo{
      img{
        width: 75%;
      }
    }

    .nav-bar{
      display: flex;
      font-size: 14px;
      column-gap: 10px;
    }
  }

</style>
