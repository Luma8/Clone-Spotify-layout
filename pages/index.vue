<template>
  <!-- <Tutorial/> -->
  <div class="main">
    <div class="d-flex">
      <left-menu/>
      <home-page/>
      <footer-menu/>
    </div>
  </div>
</template>
<script>
import HomePage from '../components/templates/HomePage'
import LeftMenu from '../components/templates/LeftMenu'
import FooterMenu from '../components/templates/FooterMenu'

export default {
  components: { HomePage, LeftMenu, FooterMenu },
  name: 'IndexPage'
}
</script>
<style scoped>
.main {
  background-color: #121212;
  height: 100vh;
  width: 100vw;
}
</style>