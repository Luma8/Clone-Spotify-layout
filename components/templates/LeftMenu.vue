<template>
  <div class="left-menu-content">
    <div class="container">
      <a href="/">
        <img class="logo-style mt-4 ml-2" src="/Logo/SpotifyLogo.png"/>
      </a>
      <div>
        <left-menu-links/>
      </div>
    </div>
  </div>
</template>
<script>
import LeftMenuLinks from '../organisms/LeftMenuLinks.vue'

export default {
  components: { LeftMenuLinks }
}
</script>
<style scoped>
.left-menu-content {
    background-color: black;
    width: 372px;
    height: 100vh;
}
.logo-style {
  width: 131px;
}
</style>
