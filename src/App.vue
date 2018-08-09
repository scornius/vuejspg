<template>
  <div id="app">
    <h1>Vue.js</h1>
    <router-view/>

<!--
<Hello/>
<FancyLabel title="Fancy Headline"/>
<MyLink/>
<CoinFlip/>
<DiceRoll/>
<EnterYourName/>
<ChooseYourGender/>
<SelectYourHobbies/>
-->

    <Parent v-on:myevent="console.log('soso')"/>

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
import FancyLabel from './components/FancyLabel'
import Parent from './components/Parent'

export default {
  name: 'App',
  components: {
    Parent,
    FancyLabel,
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
