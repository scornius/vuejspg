<template>
  <div id="app">
    <h1>Vue.js</h1>
    <router-view/>

<!--
<Hello/>
<MyLink/>
<CoinFlip/>
<DiceRoll/>
<EnterYourName/>
-->

    <ChooseYourGender/>

  </div>
</template>

<script>
import Hello from './components/HelloWorld'
import MyLink from './components/MyLink'
import CoinFlip from './components/CoinFlip'
import DiceRoll from './components/DiceRoll'
import EnterYourName from './components/EnterYourName'
import ChooseYourGender from './components/ChooseYourGender'

export default {
  name: 'App',
  components: {
    ChooseYourGender,
    EnterYourName,
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
