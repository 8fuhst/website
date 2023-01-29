<template>
  <div class="ms-3 mt-5">
    <IntroductionBlock/>
  </div>
</template>


<script>
import "bootstrap/dist/css/bootstrap.min.css"
import "bootstrap"
import IntroductionBlock from "@/components/IntroductionBlock";

export default {
  name: 'App',
  components: {
    IntroductionBlock,
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
  margin-top: 60px;
}
</style>
