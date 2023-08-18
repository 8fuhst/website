<template>
  <div :style="{ fontSize: 72 + 'px'}" class="flex first">
    <GothicVueWriter :array="['Hello, World!']" :typeSpeed="80" :iterations="1" />
  </div>
  <div :style="{ fontSize: 72 + 'px'}" class="flex second">
    <GothicVueWriter :array="['Jeg er Noah!', 'I\'m Noah!', 'Ich bin Noah!']" :typeSpeed="80"
                     :start="2500"/>
  </div>
  <div :style="{ fontSize: 34 + 'px'}" class="flex who-am-i">
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
.first {
  margin-top: 100px;
}
.second {
  margin-top: -40px;
}
.who-am-i {
  margin-top: -10px;
  font-family: "Quicksand", sans-serif;
  line-height: 40px;
  color: #a7a8a7;
}
</style>