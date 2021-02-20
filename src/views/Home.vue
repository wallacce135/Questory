<template>
  <header>
    <div class="container">
      <span><h1>Q</h1></span>
    </div>
  </header>
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
</script>

<style lang="scss">
header {
  height: 85px;
  width: 100%;
  background: #9ED186;
}
.container {
  width: calc(100vw / 1.6);
  margin: 0 auto;
  display: flex;
}
.logo a {
  font-size: 64px;
  font-family: Combay;
  text-decoration: none;
}
ul {
  list-style: none;
}
.categories li {
  display: inline;
  padding: 0 0 0 20px;
}
</style>
