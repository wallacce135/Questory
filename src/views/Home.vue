<template>
  <Header></Header>
  <main class="container">
    <Search></Search>
    <ul class="categories">
      <li><a href="#">Начатые</a></li>
      <li><a href="#">Законченные</a></li>
    </ul>
  </main>
</template>

<script>
import Header from '.././components/Header.vue'
import Search from '.././components/Search.vue'

export default {
  name: 'Home',
  components: {
    Header,
    Search
  }
}
</script>

<style lang="scss">
* {
  font-family: Gilroy;
}
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
