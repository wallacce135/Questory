<template>
  <!-- <div id="nav">
    <router-link class="link" to="/">Home</router-link> |
    <router-link class="link" to="/about">About</router-link>
  </div> -->
  <router-view/>
</template>
<style lang="scss">
  *{
    margin: 0;
    padding: 0;
  }
  #nav{
    text-align: center;
    background: #9ED186;
  }
  .link
  {
    text-decoration: none;
  }
</style>
