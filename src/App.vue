<template>
  <div id="app">
    <presentation></presentation>
    <about></about>
    <skills></skills>
  </div>
</template>

<script>
import Presentation from './views/Presentation.vue';
import About from './views/About.vue';
import Skills from './views/Skills.vue';

export default {
  name: 'app',
  components: {
    Presentation,
    About,
    Skills
  }
}
</script>

<style lang="scss">
</style>
