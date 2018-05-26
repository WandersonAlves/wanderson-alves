<template>
  <div id="app">
    <presentation></presentation>
    <about></about>
  </div>
</template>

<script>
import Presentation from './views/Presentation.vue';
import About from './views/About.vue';

export default {
  name: 'app',
  components: {
    Presentation,
    About
  }
}
</script>

<style lang="scss">
</style>
