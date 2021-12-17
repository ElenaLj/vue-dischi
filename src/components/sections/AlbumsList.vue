<template>
    <div class="albumslist">
        <SelectGenre @genre="searchGenre"/>
        <div class="container">
            <div class="albums-container" v-for="(album, index) in filteredGenres" :key="index">
                <AlbumCard :info="album"/>
            </div>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
import AlbumCard from '../commons/AlbumCard.vue';
import SelectGenre from '../commons/SelectGenre.vue';

export default {
    name: 'AlbumsList',
    components: {
        AlbumCard,
        SelectGenre
    },
    data(){
        return {
            albums: [],
            searchSong: ""
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
    },
    methods: {
        searchGenre(genre) {
            console.log(genre);
            this.searchSong = genre;
        }
    },
    computed: {
        filteredGenres() {
            console.log(this.albums, this.searchSong);
            return this.albums.filter((el) =>{
                return el.genre.toLowerCase().includes(this.searchSong);
            });
        },
    },
}
</script>

<style lang="scss" scoped>

    .albums-container {
        width: calc(100% / 5 - 20px);
    }
    
</style>