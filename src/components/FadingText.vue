<template>
  <transition name="fade" appear>
    <p>A Software Developer <br> from Germany</p>
  </transition>
</template>

<script>
export default {
  name: "FadingText",
}
</script>

<style scoped>
  .fade-enter-active {
    transition: opacity 3s ease;
  }
  .fade-enter-from {
    opacity: 0;
  }
</style>