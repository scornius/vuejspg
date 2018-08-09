<template>
  <div>
    <span>I got: {{myValue}}</span>
    <Child v-on:myevent="setValue($event)"/>
  </div>
</template>

<script>
import Child from './Child'
export default {
  name: 'Parent',
  components: {Child},
  data () {
    return {
      myValue: 'nothing'
    }
  },
  methods: {
    setValue (val) {
      this.myValue = val
    }
  }
}
</script>

<style scoped>

</style>
