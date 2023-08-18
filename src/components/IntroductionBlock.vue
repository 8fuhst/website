<template>
  <GothicVueWriter class="text-7xl" :array="['Hello, World!']" :typeSpeed="80" :iterations="1" />
  <GothicVueWriter class="text-7xl" :array="['I\'m Noah.']" :typeSpeed="80" :iterations="1"
                     :start="2500"/>
  <FadingText class="text-4xl who-am-i"/>
</template>

<script>
import GothicVueWriter from "@/components/GothicVueWriter";
 import FadingText from "@/components/FadingText";
export default {
  name: "IntroductionBlock",
  components: {
    GothicVueWriter,
    FadingText,
  }
}
</script>

<style scoped>
.fade-enter-active {
  transition-delay: 4s;
}
.who-am-i {
  font-family: "Quicksand", sans-serif;
  line-height: 40px;
  color: #a7a8a7;
}
</style>