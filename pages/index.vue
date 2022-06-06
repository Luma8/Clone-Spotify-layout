<template>
  <!-- <Tutorial/> -->
  <div class="main">
    <div class="d-flex">
      <left-menu/>
      <div>
        <navbar/>
        <home-page/>
      </div>
      <friend-list/>
    </div>
    <footer-menu/>
  </div>
</template>
<script>
import HomePage from '../components/templates/HomePage'
import LeftMenu from '../components/templates/LeftMenu'
import FooterMenu from '../components/templates/FooterMenu'
import Navbar from '../components/templates/Navbar'
import FriendList from '../components/templates/FriendList'

export default {
  components: { HomePage, LeftMenu, FooterMenu, Navbar, FriendList},
  name: 'IndexPage',
  props: {
    dark: true,
    light: false
  }
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