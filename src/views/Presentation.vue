<template>
  <div class="container flex flex-align-center flex-justify-center">
    <div class="flex flex-column padding">
      <p class="line-1">HELLO</p>
      <div class="translate-box-1">
        <p class="line-2">Wanderson Alves</p>
        <div class="translate-box-2">
          <p class="line-3">Developer, Designer, Enthusiast.</p>
          <div class="flex flex-justify-end">
            <p class="line-4">And other things that you should know...</p>
          </div>
        </div>
      </div>
    </div>
    <avatar></avatar>
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
  background: linear-gradient(359deg, #1c0f0f, #290000, #1c0f0f);
  background-size: 600% 600%;
  animation: GradientAnimation 25s ease infinite;
  width: 100vw;
  height: 100vh;
  letter-spacing: .01em;
  box-sizing: border-box;
  border: 5px solid white;
  box-shadow: inset 0px 0px 76px 0px rgba(255,255,255,0.25);

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
.translate-box-1 {
  transform: translateY(-50px);
  @media (max-width: 768px) {
    transform: unset;
  }
}
.translate-box-2 {
  transform: translateY(-10px);
  @media (max-width: 768px) {
    transform: unset;
  }
}
.line-1 {
  color: rgba(255,255,255,0.35);
  font-size: 4em;
  overflow: unset;
}
.line-2 {
  color: #f1f1f1;
  font-size: 2em;
  overflow: unset;
  letter-spacing: 3px;
  font-weight: 300;
}
.line-3 {
  color: #f1f1f1;
  letter-spacing: 0.2em;
  overflow: unset;
}
.line-4 {
  color: rgba(255,255,255,0.2);
  font-style: italic;
  overflow: hidden;
  font-size: 0.9em;
}

.padding {
  padding: 20px;
}
@keyframes GradientAnimation {
  0%{background-position:50% 0%}
  50%{background-position:50% 100%}
  100%{background-position:50% 0%}
}
</style>


