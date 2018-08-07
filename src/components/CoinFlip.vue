<template>
    <div>
      <span v-if="heads">Heads</span>
      <span v-else>Tails</span>
    </div>
</template>

<script>
export default {
  name: 'CoinFlip',
  data () {
    return {
      heads: Math.random() > 0.5
    }
  }
}
</script>

<style scoped>

</style>
