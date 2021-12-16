<template>
  <div class="albums-container">
        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div class="text">
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>

        <div class="album">
            <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="Bon Jovi, New Jersey Album">
            <h3>New Jersey</h3>
     
            <div>
                <p>Bon Jovi</p>
                <p>1988</p>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: 'AlbumCard'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

   .album {
            width: calc(100% / 5 - 20px);
            height: 300px;
            padding: 10px;
            margin-bottom: 10px;
            background-color: $background-lightblue;
            text-align: center;
            

            img {
                width: 80%;
                border-radius: 5px;
            }

            .text {
                margin-top: 10px;
            }
        }

</style>