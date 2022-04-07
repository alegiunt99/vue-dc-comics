<template>
  <main class="main-page">
    <!-- Jumbotron -->
    <div class="jumbotron">
    </div>

    <!-- Parte centrale con le card de i fumetti -->
    <div class="container">
      <section id="central-section">
        
      </section>
    </div>
  </main>
</template>

<script>
export default {
  name: 'MainApp',
  
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
