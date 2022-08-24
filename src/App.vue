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
#app {

}
</style>
