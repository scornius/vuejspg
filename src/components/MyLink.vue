<template>
    <div>
      <a v-bind:href="url">click me</a><br/>
      <a :href="url">click me</a>
    </div>
</template>

<script>
export default {
  name: 'MyLink',
  data () {
    return {
      url: 'http://vuejs.org'
    }
  }
}
</script>

<style scoped>

</style>
