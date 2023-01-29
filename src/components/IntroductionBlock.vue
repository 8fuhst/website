<template>
  <div :style="{ fontSize: 84 + 'px'}" class="flex first">
    <GothicVueWriter :array="['Hello, World!']" :typeSpeed="80" :iterations="1" />
  </div>
  <div :style="{ fontSize: 84 + 'px'}" class="flex second">
    <GothicVueWriter :array="['Jeg er Noah!'/*, 'I\'m Noah!', 'Ich bin Noah!'*/]" :iterations="1" :typeSpeed="80"
                     :start="2500"/>
  </div>
  <div :style="{ fontSize: 42 + 'px'}" class="flex who-am-i">
    <FadingText/>
  </div>
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
</style>