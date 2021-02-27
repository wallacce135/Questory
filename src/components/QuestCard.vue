<template>
    <figure class="quest-preview" v-on:click="display">
          <img src="/img/greenBack.png">
          <figcaption>
            <span>Квест1</span>
            <p>Какое-то описание</p>
          </figcaption>
          <PopQuest></PopQuest>
        </figure>
</template>

<script>
import PopQuest from '.././components/PopQuest.vue'

export default {
  name: 'QuestCard',
  components: {
    PopQuest
  }
}
</script>
