<template>
  <main>
      <AlbumsList/>
  </main>
</template>

<script>
import AlbumsList from '../sections/AlbumsList.vue';

export default {
    name: 'Main',
    components: {
        AlbumsList
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    main {
        height: calc(100vh - 70px);
        position: relative;
        background-color: $background-darkblue;
    }
</style>