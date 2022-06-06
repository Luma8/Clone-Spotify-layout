<template>
    <footer class="footer-menu dark d-flex align-items-center">
        <div class="w-25 song-content d-flex align-items-center">
            <img class="music-wp mr-2" src="../../assets/static/katebush.png" alt="">
            <div>
                <div class="d-flex align-items-center">
                    <span class="music-fs mr-2">Running Up That Hill (A deal With God)</span>
                    <fa :icon="['fas', 'heart']" />
                </div>
                <span class="music-fs-low">Kate Bush</span>
            </div>
        </div>
        <div class="w-50 d-flex justify-content-center">
            <audio controls src=""></audio>
        </div>
        <div class="w-25 text-right">
            <button class="mr-5 button-chat">
                <fa class="text-white" :icon="['fas', 'comment']" />
            </button>
        </div>
    </footer>
</template>
<script>
export default {
    props: {
        dark: true
    }
}
</script>
<style scoped>
.footer-menu {
    width: 100%;
    padding: 2.5% 0%;
    position: fixed;
    bottom: 0;
    height: 8vh;
}
.music-fs {
    font-size: 12px
}
.music-fs-low {
    font-size: 9px
}
.music-wp {
    width: 70px;
    height: 70px;
}
.dark {
    background-color: #181818;
    color: white;
}
.light {
    background-color: white;
    color: black
}
.slider-style {
    background-color: white;
}
.button-chat {
    background: linear-gradient(45deg, #3c93d1, #104b80, #1d125c, #5f57b1);
    padding: 2% 2%;
    border-radius: 100%;
    line-height: 20px;
    font-size: 25px;
}
</style>
