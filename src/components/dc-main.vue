<template>
  <div class="dc-main">
    <div class="Jumbo">
      <img class="Jumbo" src="../assets/img/jumbotron.jpg">
    </div>
    <dc-comics />
  </div>
</template>

<script>
import dcComics from './dc-comics.vue'

export default {
  components: { dcComics },
     name: 'DCmain'
}
</script>

<style scoped lang="scss">

.dc-main {

    color:white;
    background-color: #1A1A1A;
    

    .Jumbo{
      width: 100%;
      height:300px;
      overflow: hidden;
      
      
      img {
        width: 100%;
        object-fit: cover;
        object-position: top;
        

      }

      h2 {

        font-size: 50px;
      }
    }
}

</style>