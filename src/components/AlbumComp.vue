<template>
  <div class="albumCard">
    <img :src="album.poster" alt="" />
    <h5 class="title">{{ album.title.toUpperCase()}}</h5>
    <p class="author">{{ album.author }}</p>
    <p class="year">{{ album.year }}</p>
  </div>
</template>

<script>
export default {
  name: "AlbumComp",
  props: {
    album: Object,
  },
};
</script>

<style lang="scss" scoped>
.albumCard {

  width: calc(90% / 5);
  background-color: #2d3a46;
  padding: 2rem;
  text-align: center;
  margin-top: 30px;

  img {
    width: 200px;
    height: 200px;
    margin-bottom: 1rem;
  }

  p{
    background-color: #2d3a46;
    margin-bottom: 0px;
    color: gray;
  }

  h5{
    background-color: #2d3a46;
    color: white;
    margin-bottom: 2rem;
  }
}
</style>
