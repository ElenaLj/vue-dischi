<template>
        <div class="album">
            <img :src="info.poster" :alt="info.author">
            <h3>{{info.title}}</h3>
     
            <div class="text">
                <p>{{info.author}}</p>
                <p>{{info.year}}</p>
            </div>
        </div>
</template>

<script>
export default {
    name: 'AlbumCard',
    props:  {
        info: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

   .album {
        height: 300px;
        padding: 10px;
        margin-bottom: 20px;
        background-color: $background-lightblue;
        text-align: center;
            

            img {
                width: 80%;
                border-radius: 5px;
            }

            .text {
                margin-top: 10px;
                color: $text-grey;
            }
    }

</style>