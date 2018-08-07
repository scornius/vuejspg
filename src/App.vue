<template>
  <div id="app">
    <h1>Vue.js</h1>
    <router-view/>

<!--
<Hello/>
<MyLink/>
<CoinFlip/>
-->

    <DiceRoll/>

  </div>
</template>

<script>
import Hello from './components/HelloWorld'
import MyLink from './components/MyLink'
import CoinFlip from './components/CoinFlip'
import DiceRoll from './components/DiceRoll'

export default {
  name: 'App',
  components: {
    DiceRoll,
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
