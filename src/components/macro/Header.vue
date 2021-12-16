<template>
  <header>
      <img src="../../assets/img/spotify-logo-small.png" alt="the Spotify logo">
  </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    header {
        height: 70px;
        width: 100vw;
        padding: 10px 0;
        background-color: $background-lightblue;

        img {
            max-height: 50px;
        }
    }
</style>