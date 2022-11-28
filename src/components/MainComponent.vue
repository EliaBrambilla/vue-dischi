<template>
  <div id="container" v-if="albumsArr.length > 9">
      <TrackComp
      v-for="(element, index) in albumsArr"
      :key="index"
      :album="element"
      />
  </div>

</template>

<script>
  import TrackComp from "./elements/TrackComp.vue"
  import axios from 'axios'
  export default {
      name: 'MainComp',
      components: {
          TrackComp
      },
      data(){
          return{
              albumsArr: []
          }
      },
      mounted(){
          this.CompileAlbums();
      },
      methods: {
          CompileAlbums(){
              axios.get('https://flynn.boolean.careers/exercises/api/array/music')
              .then((response) => {
                  this.albumsArr = response.data.response;
                  console.log(this.albumsArr)
              })
          }
      }
  }
</script>

<style lang="scss" scoped>
  #container{
      width: 75%;
      height: calc( 100% - 90px );
      margin: auto;
      padding: 40px;
      display: flex;
      justify-content: space-evenly;
      align-content: center;
      flex-wrap: wrap;
  }
</style>