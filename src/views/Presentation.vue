<template>
    <div class="container flex flex-align-center flex-justify-center">
        <avatar></avatar>
        <div class="flex flex-column padding">
            <p class="white font-montserrat">Hi, Wanderson Alves over here!</p>
            <p class="white font-montserrat">I’m a Front-End Developer & UI Designer.</p>
            <p class="white font-montserrat">Currently living in Recife, Brazil.</p>
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
  letter-spacing: .01em;
  > * {
    margin-right: 20px;
    font-size: 1.2em;
    @media (max-width: 768px) {
        margin-right: unset;
    }
  }
  @media (max-width: 768px) {
      flex-direction: column;
      text-align: center;
      line-height: 22px;
      > * {
          margin-bottom: 20px;
      }
  }  
}
.padding {
    padding: 20px;
}
@keyframes GradientAnimation { 
    0%{background-position:0% 50%}
    50%{background-position:100% 50%}
    100%{background-position:0% 50%}
}
</style>


