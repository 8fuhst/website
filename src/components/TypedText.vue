<template>
  <span ref="typing"></span>
</template>

<script>
import Typed from 'typed.js'
import {onMounted, ref} from "vue";

const typing = ref(null)
const typing_text = null

onMounted(() => {
  new Typed(typing.value, {
    strings: typing_text,
    typeSpeed: 100
  })
})
export default {
  props: {
    text: {required: true, type: String}
  }
}
</script>

<style scoped>

</style>