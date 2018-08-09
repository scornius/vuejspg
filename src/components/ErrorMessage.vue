<template>
  <div>
    An unexpected error occurred: <slot name="message"></slot><br/>
    <slot name="detail"></slot>
  </div>
</template>

<script>
export default {
  name: 'ErrorMessage'
}
</script>

<style scoped>

</style>
