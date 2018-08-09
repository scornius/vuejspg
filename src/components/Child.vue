<template>
    <div>
      <button v-on:click="sendEvent('A')">Send event A</button>
      <button @click="sendEvent('B')">Send event B</button>
    </div>
</template>

<script>
export default {
  name: 'Child',
  methods: {
    sendEvent (val) {
      this.$emit('myevent', 'something ' + val)
    }
  }
}
</script>

<style scoped>

</style>
