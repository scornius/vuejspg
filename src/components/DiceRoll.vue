<template>
    <div>
      <button v-on:click="rollDice">Roll it</button>
      <button @click="rollDice">Roll it</button>
      <span>Result: {{result}}</span>
    </div>
</template>

<script>
export default {
  name: 'DiceRoll',
  data () {
    return {
      result: 0
    }
  },
  methods: {
    rollDice () {
      this.result = Math.round(Math.random() * 6)
    }
  }
}
</script>

<style scoped>

</style>
