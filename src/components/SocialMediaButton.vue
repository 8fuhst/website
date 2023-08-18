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
    },
  }
})

</script>

<template>
  <transition name="fade" appear>
    <div class="mr-5 rounded-md scale-100 hover:scale-105 ease-in duration-150 hover:drop-shadow-md">
      <img class="rounded-lg w-8 " :src=image @click="openLink()" alt="" @mouseover="highlight"/>
    </div>
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