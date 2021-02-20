<template>
  <Header></Header>
  <main class="container">
    <div>
      <input type="text">
    </div>
    <ul class="categories">
      <li><a href="#">Начатые</a></li>
      <li><a href="#">Законченные</a></li>
    </ul>
  </main>
</template>

<script>
import Header from '.././components/Header.vue'

export default {
  name: 'Home',
  components: {
    Header
  }
}
</script>

<style lang="scss">
.container {
  width: calc(100vw / 1.6);
  margin: 0 auto;
  display: flex;
}
ul {
  list-style: none;
}
.categories li {
  display: inline;
  padding: 0 0 0 20px;
}
</style>
