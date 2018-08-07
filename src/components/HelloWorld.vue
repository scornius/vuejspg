<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h1 v-html="msg.replace('H','h')"></h1>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Hello <u>world</u> !'
    }
  }
}
</script>

<style scoped>
h1 {
  color: crimson;
}
</style>
