<template>
  <div class="flex h-full">
    <div class="grid grid-cols-2">
      <div class="grid grid-rows-3">
        <div class="ml-5 row-span-2">
          <IntroductionBlock/>
        </div>
        <div class="flex">
          <div class="ml-5 -mt-1 grid grid-cols-2 grid-rows-1">
            <SocialMediaButton class="" v-for="media in socialMedia" :media="media" :key="media"/>
          </div>
        </div>
      </div>
      <div>
        <ImageDisplay/>
      </div>
    </div>
  </div>
</template>


<script>
import "bootstrap/dist/css/bootstrap.min.css"
import "bootstrap"
import IntroductionBlock from "@/components/IntroductionBlock";
import ImageDisplay from "@/components/ImageDisplay";
import SocialMediaButton from "@/components/SocialMediaButton.vue";

export default {
  name: 'App',
  components: {
    SocialMediaButton,
    IntroductionBlock,
    ImageDisplay
  },
  created() {
    document.title = "Noah Fuhst";
    this.socialMedia = ['github', 'linkedin']
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  height: 100vh;
}
</style>
