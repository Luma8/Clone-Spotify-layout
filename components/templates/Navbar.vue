<template>
  <nav class="nav-bar container d-flex justify-content-between align-items-center">
    <div>
      <button class="button-step text-center">
        <fa :icon="['fas', 'angle-left']"/>
      </button>
      <button class="button-step text-center">
        <fa :icon="['fas', 'angle-right']"/>
      </button>
    </div>
    <div>
      <button class="profile-button d-flex justify-content-between align-items-center">
        <fa class="profile-icon" :icon="['fas', 'user-circle']"/>
        <span class="fw-bold fs-5">Lucas Matheus</span>
        <fa class="mr-2" :icon="['fas', 'caret-down']"/>
      </button>
    </div>
  </nav>
</template>
<script>
export default {
}
</script>
<style scoped>
.nav-bar {
    position: fixed;
    width: 80%;
    color: white;
}
.button-step {
  background-color: black;
  font-size: 25px;
  width: 32px;
  height: 32px;
  -webkit-box-pack: center;
  -webkit-box-align: center;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  opacity: .6;
  position: relative;
  margin-right: 16px;
}
.profile-button {
  background-color: black;
  width: 180px;
  border-radius: 20px;
}
.profile-icon {
  height: 30px;
  width: 30px;
}
</style>
