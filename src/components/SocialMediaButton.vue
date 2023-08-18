<script>
import {defineComponent} from 'vue'

export default defineComponent({
  name: "SocialMediaButton",
  props: ['media'],
  data() {
    return {
      image: undefined,
      link: undefined
    }
  },
  created() {
    if (this.media === "github") {
      this.image = require("./images/github.png")
      this.link = "https://www.github.com/8fuhst"
    }
    else if (this.media === "linkedin") {
      this.image = require("./images/linkedin.png")
      this.link = "https://www.linkedin.com/in/noah-fuhst/"
    }
  },
  methods: {
    openLink() {
      window.open(this.link)
    }
  }
})

</script>

<template>
  <transition name="fade" appear>
    <img class="w-8 mr-5" :src=image @click="openLink()" alt=""/>
  </transition>
</template>

<style scoped>
.fade-enter-active {
  transition: opacity 3s ease;
  transition-delay: 4s;
}
.fade-enter-from {
  opacity: 0;
}
</style>