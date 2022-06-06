<template>
    <div class="left-menu-content">
        <div class="container">
            <div class="d-flex justify-content-between align-items-center text-white">
                <span>Friend Activy</span>
                <fa :icon="['fas', 'user-plus']" />
            </div>
            <div class="mt-4" v-for="sims in friend" :key="'amigos'+sims">
                <div class="text-white d-flex align-items-center container-friends">
                    <fa class="profile-icon profile-icon mr-2" :icon="['fas', 'user-circle']"/>
                    <div class="w-100">
                        <div class="d-flex justify-content-between align-items-center">
                            <span class="name-friend">{{ sims.name }}</span>
                            <span class="description-friend">{{ sims.action_timer }}</span>
                        </div>
                        <div>
                            <span class="description-friend">{{ sims.artist }}</span>
                            <span class="description-friend">{{ sims.song }}</span>
                            <div>
                                <span class="description-friend">{{ sims.plalist_friend }}</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import LeftMenuLinks from "../organisms/LeftMenuLinks.vue";

export default {
    components: { LeftMenuLinks },
    data () {
        return {
            friend: [
                { name: 'User-1', artist: 'Kate Bush', song: 'Running...', plalist_friend: 'Mix day 3', action_timer: '5min' },
                { name: 'user-2', artist: 'Linkin Park', song: 'Running...', plalist_friend: 'Mix day 3', action_timer: '5min' },
                { name: 'user-23', artist: 'Metalica', song: 'Running...', plalist_friend: 'Mix day 3', action_timer: '5min' },
                { name: 'user-32', artist: 'Red Hot...', song: 'Running...', plalist_friend: 'Mix day 3', action_timer: '5min' } 
            ]
        }
    }
}
</script>
<style scoped>
.left-menu-content {
    background-color: black;
    width: 270px;
    height: 100vh;
}
.container-friends {
    overflow-y: scroll;
}
.profile-icon {
    font-size: 40px;
}
.description-friend {
    font-size: 10px;
}
</style>
