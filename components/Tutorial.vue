<!-- Please remove this file from your project -->
<template>
  <div class="index-main">
    <h1>Esse é o index-main / Tutorial</h1>
    <FormMain />
  </div>
</template>
<style>
.index-main {
  padding: 10px;
  background-color: #c76a07;
  text-align: center;
}
</style>
<script>
import FormMain from './FormMain'
export default {
  name: 'NuxtTutorial',
  components: {
    FormMain
  }
}
</script>
