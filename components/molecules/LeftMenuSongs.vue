<template>
    <div class="menu-songs">
        <div class="mt-2 menu-songs-content ml-2" v-for="song in songs" :key="'Songs'+song" >
            <a class="links-songs" href="#">
                {{ song.tracks }}
            </a>
        </div>
    </div>
</template>
<script>
export default {
    data () {
        return {
            //MOckups
            songs : [
                { tracks: 'Kate Bush'}, 
                { tracks: 'Song-2'},
                { tracks: 'Song-3'},
                { tracks: 'Song-4'}, 
                { tracks: 'Song-5'},
                { tracks: 'Song-6'},
                { tracks: 'Song-7'}, 
                { tracks: 'Song-8'},
                { tracks: 'Song-9'},
                { tracks: 'Song-10'}, 
                { tracks: 'Song-11'},
                { tracks: 'Song-12'},
                { tracks: 'Song-13'}, 
                { tracks: 'Song-14'},
                { tracks: 'Song-15'},
                { tracks: 'Song-16'},
                { tracks: 'Song-17'},
                { tracks: 'Song-18'},
                { tracks: 'Song-19'},
                { tracks: 'Song-20'},
                { tracks: 'Song-21'},
                { tracks: 'Song-22'},
                { tracks: 'Song-23'},
                { tracks: 'Song-24'},
                { tracks: 'Song-25'},
                { tracks: 'Song-26'},
                { tracks: 'Song-27'},
                { tracks: 'Song-28'},
                { tracks: 'Song-29'},
                { tracks: 'Song-30'},
                { tracks: 'Song-31'},
            ]
        }
    },
}
</script>
<style scoped>
.menu-songs {
    border-top: 1px solid rgb(44, 43, 43);
    height: 530px;
    overflow-y: scroll;
}
.links-songs {
    color: #b3b3b3;
    text-decoration: none;
}
.links-songs:hover {
    color: white;
    transition: all 0.2s ease-in;
}
</style>
