<template>
 <div class="dc-header">
     <div class="head-logo">
         <img src="../assets/img/dc-logo.png" alt="DC Comics Logo">
     </div>
     <div class="nav">
         <ul v-for="(link, index) in links" :key="index">
             <li><a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a></li>
         </ul>
     </div>
 </div>
</template>

<script>
export default {

    name: 'DCheader',
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    active: false
                },

                {
                    text: 'Comics',
                    url: '#',
                    active: true
                },

                {
                    text: 'Movies',
                    url: '#',
                    active: false
                },
                {
                    text: 'TV',
                    url: '#',
                    active: false
                },

                {
                    text: 'Games',
                    url: '#',
                    active: false
                },

                {
                    text: 'Collectibles',
                    url: '#',
                    active: false
                },

                {
                    text: 'Videos',
                    url: '#',
                    active: false
                },

                {
                    text: 'Fans',
                    url: '#',
                    active: false
                },

                {
                    text: 'News',
                    url: '#',
                    active: false
                },

                {
                    text: 'Shop',
                    url: '#',
                    active: false
                },
            ]
        }
    }
}


</script>

<style lang="scss">

</style>