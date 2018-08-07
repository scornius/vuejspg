<template>
  <div>
    <select v-model="selectedHobbies" multiple>
      <option v-for="option in hobbies" v-bind:key="option.value" >
        {{ option.text }}
      </option>
    </select>
    <br/>
    <span>{{selectedHobbies}}</span>
  </div>
</template>

<script>
export default {
  name: 'SelectYourHobbies',
  data () {
    return {
      hobbies: [
        { text: 'Fencing', value: 'A' },
        { text: 'Paragliding', value: 'B' },
        { text: 'Skydiving', value: 'C' }
      ],
      selectedHobbies: []
    }
  }
}
</script>

<style scoped>

</style>
