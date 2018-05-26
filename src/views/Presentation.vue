<template>
    <div class="container flex flex-align-center flex-justify-center">
        <avatar></avatar>
        <div class="flex flex-column font-montserrat">
            <span>Hi, Wanderson Alves over here!</span>
            <span>I’m a Front-End Developer & UI Designer.</span>
            <span>Currently living in Recife, Brazil.</span>
        </div>
    </div>
</template>
<script>
import Avatar from '@/components/Avatar.vue';

export default {
    name: 'Presentation',
    components: {
        Avatar
    }
}
</script>
<style lang="scss" scoped>
.container {
  background: linear-gradient(270deg, #f4376d, #66349d);
  background-size: 400% 400%;
  animation: GradientAnimation 25s ease infinite;
  width: 100vw;
  height: 100vh;
}
@keyframes GradientAnimation { 
    0%{background-position:0% 50%}
    50%{background-position:100% 50%}
    100%{background-position:0% 50%}
}
</style>


