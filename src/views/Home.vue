<template>
  <Header></Header>
  <main class="container">
    <div class="two-col">
      <Search></Search>
      <ul class="categories">
        <li><a href="#">Начатые</a></li>
        <li><a href="#">Законченные</a></li>
      </ul>
    </div>
    <div id="quests" class="two-col">
        <figure class="quest-preview">
          <img src="/img/greenBack.png">
          <figcaption>
            <span>Квест1</span>
            <p>Какое-то описание</p>
          </figcaption>
        </figure>
    </div>
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
  .two-col {
    display: flex;
    justify-content: space-between;
    width: 100%;
    align-items: center;
  }
  .quest-preview {
    width: calc(40%);
    background: #FFFFFF;
    box-shadow: 0px 4px 16px rgba(0, 0, 0, 0.07);
    border-radius: 10px;
    overflow: hidden;
    height: 267px;
    img {
      width: calc(100% - 26px);
      padding: 13px;
    }
    span {
      font-size: 20px;
      font-weight: bold;
    }
    figcaption {
      padding-left: 20px;
    }
  }
}
.container > div {
  margin-top: 40px;
}
ul {
  list-style: none;
}
.categories li {
  display: inline;
  padding: 0 0 0 20px;
}
</style>
