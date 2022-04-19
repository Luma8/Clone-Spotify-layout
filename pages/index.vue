<template>
  <!-- <Tutorial/> -->
  <div class="main">
    <div class="d-flex">
      <left-menu/>
      <div>
        <navbar/>
        <home-page/>
      </div>
    </div>
    <footer-menu/>
  </div>
</template>
<script>
import HomePage from '../components/templates/HomePage'
import LeftMenu from '../components/templates/LeftMenu'
import FooterMenu from '../components/templates/FooterMenu'
import Navbar from '../components/templates/Navbar.vue'

export default {
  components: { HomePage, LeftMenu, FooterMenu, Navbar },
  name: 'IndexPage'
}
</script>
<style scoped>
.main {
  background-color: #121212;
  height: 100vh;
  width: 100vw;
  overflow-y: hidden;
}
</style>