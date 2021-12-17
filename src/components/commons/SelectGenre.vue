<template>
  <div class="select-genre">
      <label for="genre">Choose your favourite music genre:</label>
      <select name="genre-selection" id="genre" v-model="selectGenre" @change="$emit('genre', selectGenre)">
          <option value="rock">Rock</option>
          <option value="pop">Pop</option>
          <option value="jazz">Jazz</option>
          <option value="metal">Metal</option>
      </select>
  </div>
</template>

<script>
export default {
    name: 'SelectGenre',
    data(){
        return {
            selectGenre: ""
        } 
    }
}
</script>

<style lang="scss" scoped>

</style>