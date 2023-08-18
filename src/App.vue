<template>
  <div class="flex">
    <div class="grid grid-cols-2">
      <div class="grid grid-rows-5">
        <div class="ml-5 row-span-3">
          <IntroductionBlock/>
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

export default {
  name: 'App',
  components: {
    IntroductionBlock,
    ImageDisplay
  },
  created() {
    document.title = "Noah Fuhst";
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
}
</style>
