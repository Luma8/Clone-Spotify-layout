<template>
  <div class="mt-4">
      <div class="mb-3 ml-2">
        <a href="#" class="link-color">
            <fa class="icon-size mr-3" :icon="['fas', 'home-alt']"/>
            <span>Home</span>
        </a>
      </div>
      <div class="mb-3 ml-2">
        <a href="#" class="link-color">
            <fa class="icon-size mr-3" :icon="['fas', 'search']"/>
            <span>Search</span>
        </a>
      </div>
      <div class="mb-3 ml-2">
        <a href="#" class="link-color">
            <fa class="icon-size mr-3" :icon="['fas', 'book']"/>
            <span>Your Library</span>
        </a>
      </div>
      <div class="mt-5">
        <div class="mb-3 ml-2">
            <a href="#" class="link-color">
                <fa class="icon-size mr-3" :icon="['fas', 'plus-square']"/>
                <span>Create playlist</span>
            </a>
        </div>
        <div class="mb-3 ml-2">
            <a href="#" class="link-color">
                <fa class="icon-size mr-3" :icon="['fas', 'heart']"/>
                <span>Liked Songs</span>
            </a>
        </div>
        <div class="mb-3 ml-2">
          <button :class="{'toggle-button' : toggle === true, 'toggle-button-light' : toggle === false}" @click="toggleFunc()">
            <span class="button-inside" />
          </button>
          <span class="link-color ml-2">Dark</span>
        </div>
      </div>
      <left-menu-songs/>
  </div>
</template>
<script>
import LeftMenuSongs from '../molecules/LeftMenuSongs.vue'
export default {
  components: { LeftMenuSongs },
  data () {
    return {
      toggle: true
    }
  },
  methods: {
    toggleFunc () {
      this.toggle = !this.toggle
    }
  }
}
</script>
<style scoped>
.link-color {
    color: #b3b3b3;
    text-decoration: none;
    font-size: 0.876rem;
    line-height: 1rem;
    text-transform: none;
    letter-spacing: normal;
    font-weight: bold;
}
.link-color:hover{
    color: white;
    transition: all 0.2s ease-in;
}
.icon-size {
    font-size: 23px;
}
.toggle-button {
  border: 1px solid #b3b3b3;
  width: 50px;
  text-align: left;
  border-radius: 50px;
}
.toggle-button-light {
  border: 1px solid #b3b3b3;
  width: 50px;
  text-align: right;
  border-radius: 50px;
}
.button-inside {
  background-color: #b3b3b3;
  margin: 0px 2px;
  padding: 0px 10px;
  border-radius: 50px;
}
</style>