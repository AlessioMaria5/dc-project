<template>
  <div id="app">
   
    <DcHeader/>
    <DcMain/>
    <DcShop />
    <DcFooter />
  </div>
</template>

<script>
import DcHeader from "./components/dc-header.vue";
import DcMain from "./components/dc-main.vue";
import DcShop from "./components/dc-shop.vue";
import DcFooter from "./components/dc-footer.vue";


export default {
  name: 'App',
  components: {
    DcHeader,
    DcMain,
    DcShop,
    DcFooter
}
}
</script>

<style lang="scss">
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }

#app {
    h1,h2,h3,h4, .nav {

      text-transform: uppercase;

    }
}
</style>
