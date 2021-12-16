<template>
    <div class="container">
        <div class="albums-container" v-for="(album, index) in albums" :key="index">
            <AlbumCard :info="album"/>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
import AlbumCard from '../commons/AlbumCard.vue';

export default {
    name: 'AlbumsList',
    components: {
        AlbumCard
    },
    data(){
        return {
            albums: null
        }
    },
    created() {
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response) => {
        // handle success
        // console.log(response.data.response);
        this.albums = response.data.response;
        })
        .catch(function (error) {
            // handle error
            console.log(error);
        });
    }
}
</script>

<style lang="scss" scoped>

    .albums-container {
        width: calc(100% / 5 - 20px);
    }
    
</style>