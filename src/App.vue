<template>
  <div class="ms-3 mt-5">
    <div :style="{ fontSize: 84 + 'px'}" class="flex first">
      <GothicVueWriter :array="['Hello, World!']" :typeSpeed="80" :iterations="1" />
    </div>
    <div :style="{ fontSize: 84 + 'px'}" class="flex second">
      <GothicVueWriter :array="['Jeg er Noah.'/*, 'I\'m Noah!', 'Ich bin Noah!'*/]" :iterations="1" :typeSpeed="80"
                       :start="3000"/>
    </div>
    <div :style="{ fontSize: 42 + 'px'}" class="flex who-am-i">
      <!--<FadingText :start="0" :content="['A Software Developer <br> from Germany']" /-->
      <p>
        A Software Developer <br> from Germany
      </p>
    </div>
  </div>
</template>


<script>
import GothicVueWriter from "@/components/GothicVueWriter";
//import FadingText from "@/components/FadingText";
import "bootstrap/dist/css/bootstrap.min.css"
import "bootstrap"

export default {
  name: 'App',
  components: {
    GothicVueWriter,
    //FadingText
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
.first {
  margin-top: 100px;
}
.second {
  margin-top: -50px;
}
.who-am-i {
  margin-top: -10px;
  font-family: "Quicksand", sans-serif;
  line-height: 40px;
  color: #a7a8a7;

}
</style>
