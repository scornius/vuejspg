<template>
  <div id="app">
    <h1>Vue.js</h1>
    <router-view/>

    <Hello/>
<!--
   <MyLink/>
   <CoinFlip/>
-->

  </div>
</template>

<script>
import Hello from './components/HelloWorld'
import MyLink from './components/MyLink'
import CoinFlip from './components/CoinFlip'

export default {
  name: 'App',
  components: {
    CoinFlip,
    MyLink,
    Hello
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #0da006;
  margin-top: 60px;
}
</style>
