<template>
  <main class="main-page">
    <div class="container">
      <section id="central-section">
        <h3>--> Content goes here </h3>
      </section>
    </div>
  </main>
</template>

<script>
export default {
  name: 'MainApp',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.main-page{
  padding: 40px 0px;
  color: white;
  background-color: rgb(28 28 28);
}

</style>
