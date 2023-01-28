<template>
  <VueWriter />
</template>

<script>
import VueWriter from "vue-writer";

export default {
  name: "GothicVueWriter",
  components: {
    VueWriter,
  }
}
</script>

<style scoped>
.is-typed {
  font-family: "Playfair Display Bold", serif;
  display: flex;
  justify-content: start;
}

</style>