<template>
  <div class="flex h-full">
    <div class="grid grid-cols-2">
      <div class="grid grid-rows-3">
        <div class="ml-5 row-start-2">
          <IntroductionBlock class="content-start"/>
          <div class="flex row-start-3">
            <div class="mt-2 grid grid-cols-2">
              <SocialMediaButton class="" v-for="media in socialMedia" :media="media" :key="media"/>
            </div>
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
