<template>
  <div class="mt-4">
      <div class="mb-3 ml-2">
        <a href="#" class="link-color">
            <fa class="icon-size mr-3" :icon="['fas', 'home-alt']"/>
            <span>Início</span>
        </a>
      </div>
      <div class="mb-3 ml-2">
        <a href="#" class="link-color">
            <fa class="icon-size mr-3" :icon="['fas', 'search']"/>
            <span>Buscar</span>
        </a>
      </div>
      <div class="mb-3 ml-2">
        <a href="#" class="link-color">
            <fa class="icon-size mr-3" :icon="['fas', 'book']"/>
            <span>Sua Biblioteca</span>
        </a>
      </div>
      <div class="mt-5">
        <div class="mb-3 ml-2">
            <a href="#" class="link-color">
                <fa class="icon-size mr-3" :icon="['fas', 'plus-square']"/>
                <span>Criar playlist</span>
            </a>
        </div>
        <div class="mb-3 ml-2">
            <a href="#" class="link-color">
                <fa class="icon-size mr-3" :icon="['fas', 'heart']"/>
                <span>Músicas Curtidas</span>
            </a>
        </div>
      </div>
      <left-menu-songs/>
  </div>
</template>
<script>
import LeftMenuSongs from '../molecules/LeftMenuSongs.vue'
export default {
  components: { LeftMenuSongs }
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
</style>