<template>
  <div class="home-cards">
    <button class="button-chat">
      <fa :icon="['fas' , 'comment']" />
    </button>
  </div>
</template>
<script>
export default {
}
</script>
<style lang="scss" scoped>
.home-cards {
  height: 95%;
  width: 70vw;
  background: linear-gradient(45deg, #3c93d1, #104b80, #1d125c, #5f57b1);
  background-size: 300% 300%;
  animation: colors 15s ease infinite;
}
@keyframes colors {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
.button-chat {
  position: absolute;
  bottom: 0;
}
</style>
