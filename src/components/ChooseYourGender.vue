<template>
  <div>
    <input type="radio" id="m" v-model="gender" value="m"/>
    <label for="m">Male</label>
    <input type="radio" id="f" v-model="gender" value="f"/>
    <label for="f">Female</label>
    <br/>
    <span v-bind:class="{ pink: gender === 'f', blue: gender !== 'm' }">XXXXXXXXXX</span>
  </div>
</template>

<script>
export default {
  name: 'ChooseYourGender',
  data () {
    return {
      gender: 'm'
    }
  }
}
</script>

<style scoped>
  span.pink {
    color: pink;
  }
  span.blue {
    color: blue;
  }
</style>
