<template>
  <p v-if="visible">
    {{content[0]}}
  </p>
</template>

<script>
//import {defineProps} from "vue";
export default {
  name: "FadingText",
  props: ['content', 'start'],
  // TODO: Find out how to use props in script
  /*setup() {
    const props = defineProps({content: String, start: String})
    let visible = false;
    /*setTimeout(parseInt(props.start))
    visible = true;
    return { visible };
  }*/
}
</script>

<style scoped>

</style>