<template>
  <div id="app">
    <div id="nav">
      <router-link to="/echarts" >ECharts</router-link>
      |
      <router-link to="/shopping_cart">ShoppingCart</router-link>
      |
      <router-link to="/bitcoin">Bitcoin</router-link>
      |
      <router-link to="/news">News</router-link>
      |
      <router-link to="/todo">Todo</router-link>
      |
      <router-link v-bind:to="{name:'about',params:{text:'hello'}}">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
  export default {
  }
</script>

<style>
  #app {
    text-align: center;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;

  }

  #nav {
    padding: 30px;
    text-align: center;
  }

  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }

  #nav a.router-link-exact-active {
    color: #42b983;
  }
</style>
