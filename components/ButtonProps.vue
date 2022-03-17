<template>
  <div class="ButtonProps">
    <h1> ButtonProp</h1>
    <!-- <button style="#000">{{BtnText}}</button> -->
    <button @click="$emit('BtnGoogle')">trocar image google</button>
  </div>
</template>

<style scoped>
/* style dessa view */
</style>
<script>
export default {
  name: 'ButtonProps',
  emit: ['BtnGoogle'],
  props: {
    BtnText: {
      type: String,
      default: 'Value default',
    },
    BtnColor: {
      type: String,
      default: '#000',
    }
  }
}
</script>
