<template>
  <div class="FormMain">
    <h1  >Esse é o formMain</h1>
    <InputProps />
    <div class="Form-button">

    <ButtonProps :BtnText='TextBtn'/> <!-- dessa forma o props tbm pode ser passado como parametro -->
    </div>
    <!-- <ButtonProps BtnText="esse é o props button2"/> -->
    <div>
      <ImgProps />
    </div>

  </div>
</template>

<style scoped>
.FormMain {
  padding: 10px;
  background-color: #ed7d07;
  text-align: center;
  color: aqua;
}
.Form-button {
  padding: 10px;
  background-color: #271705;
  text-align: center;
  color: rgb(245, 245, 245);
}

</style>
<script>
import InputProps from "./InputProps"
import ButtonProps from "./ButtonProps"
import ImgProps from "./ImgProps"

export default {
    name: "FormMain",
    data() {
        return {
             TextBtn: "mudando o texto do button aqui"

        }
    },
    components: {
        InputProps,
        ButtonProps,
        ImgProps

    }
}
</script>
