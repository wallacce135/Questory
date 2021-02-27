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
        <QuestCard></QuestCard>
    </div>
  </main>
</template>

<script>
import Header from '.././components/Header.vue'
import Search from '.././components/Search.vue'
import QuestCard from '.././components/QuestCard.vue'

export default {
  name: 'Home',
  components: {
    Header,
    Search,
    QuestCard
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
    width: calc(48%);
    background: #FFFFFF;
    box-shadow: 0px 4px 16px rgba(0, 0, 0, 0.07);
    border-radius: 10px;
    overflow: hidden;
    img {
      width: calc(100% - 26px);
      padding: 13px;
    }
    span {
      font-size: 20px;
      font-weight: bold;
    }
    figcaption {
      padding: 0px 20px 20px 20px;
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
