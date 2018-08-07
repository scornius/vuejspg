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
<ChooseYourGender/>
<SelectYourHobbies/>
-->

    <SelectYourHobbies/>

  </div>
</template>

<script>
import Hello from './components/HelloWorld'
import MyLink from './components/MyLink'
import CoinFlip from './components/CoinFlip'
import DiceRoll from './components/DiceRoll'
import EnterYourName from './components/EnterYourName'
import ChooseYourGender from './components/ChooseYourGender'
import SelectYourHobbies from './components/SelectYourHobbies'

export default {
  name: 'App',
  components: {
    SelectYourHobbies,
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
  text-align: center;
  color: #0da006;
  margin-top: 60px;
}
</style>
