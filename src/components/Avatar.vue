<style scoped>
.avatar {
  width: 250px;
  height: 250px;
  background: linear-gradient(270deg, #f4376d, #66349d);
  background-size: 400% 400%;
  border-radius: 50%;
  padding: 8px;
  animation: Gradient 25s ease infinite;
}

@keyframes Gradient {
    0%{background-position:0% 4%}
    50%{background-position:100% 97%}
    100%{background-position:0% 4%}
}

</style>

<template>
    <img src="../assets/avatar.jpg" class="avatar center-block" alt="Wanderson Alves"/>
</template>

<script>
export default {
  name: 'Avatar'
}
</script>