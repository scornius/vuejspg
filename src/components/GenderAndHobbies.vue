<template>
    <div>
      <button @click="switchComponent">Switch it</button>
      <keep-alive>
        <component v-bind:is="currentComponent"></component>
      </keep-alive>
    </div>
</template>

<script>
import SelectYourHobbies from './SelectYourHobbies'
import ChooseYourGender from './ChooseYourGender'
export default {
  name: 'GenderAndHobbies',
  components: {ChooseYourGender, SelectYourHobbies},
  data () {
    return {
      currentComponent: 'SelectYourHobbies'
    }
  },
  methods: {
    switchComponent () {
      if (this.currentComponent === 'SelectYourHobbies') {
        this.currentComponent = 'ChooseYourGender'
      } else {
        this.currentComponent = 'SelectYourHobbies'
      }
    }
  }
}
</script>

<style scoped>

</style>
