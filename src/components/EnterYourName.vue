<template>
  <div>
    <input title="Name" v-model="myValue"/><br/>
    <span>Your name: {{myValue}}</span>
  </div>
</template>

<script>
export default {
  name: 'EnterYourName',
  data () {
    return {
      myValue: ''
    }
  },
  watch: {
    myValue: function (val) {
      console.log('value changed: ' + val)
    }
  }
}
</script>

<style scoped>

</style>
