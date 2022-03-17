<template>
  <div class="InputProps">
    <h1>Esse é o inputProps</h1>
    <input  :type="InputType" :name="InputName">

  </div>
</template>

<style scoped>
.InputProps {
  padding: 10px;
  background-color: #723b00;
  text-align: center;
  color: rgb(94, 255, 0);
}

</style>
<script>
export default {
  name: 'InputProps',
  props: {
    InputType: {
      type: String,
      default: 'text'
    },
    InputName: {
      type: String,
      default: 'InputName'
    }
  }
}
</script>
