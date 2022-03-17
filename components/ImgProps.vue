<template>
  <div class="ImgProps">
    <h1>props img</h1>
    <img :src="src" :alt="alt" :width="width" :height="height">
    <ButtonProps  @BtnGoogle="BtnGoogle" />
  </div>

</template>

<style scoped>
/* style dessa view */
.ImgProps {
  padding: 10px;
  text-align: center;
  align-items: center;

}


</style>
<script>
import ButtonProps from "./ButtonProps"
export default {
  name: 'ImgProps',
  components: {
    ButtonProps
  },
    data() {
        return {
             TextBtn: "mudar button"
        }
    },
  props: {
    src: {
      type: String,
      default: 'https://www.google.com.br/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png'
    },
    alt: {
      type: String,
      default: 'Imagem'
    },
    width: {
      type: String,
      default: '150px'
    },
    height: {
      type: String,
      default: '150px'
    }
  },
  methods: {
    BtnGoogle() {
      this.src = 'https://imagepng.org/wp-content/uploads/2020/04/live-480x432.png'
    }
  }
}
</script>
