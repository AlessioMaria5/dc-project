<template>
 <div class="dc-header">
     <div class="head-logo">
         <img src="../assets/img/dc-logo.png" alt="DC Comics Logo">
     </div>
     <div class="nav">
         <ul>
             <li v-for="(link, index) in links" :key="index" :class="link.active==ciao?'active': '' ">
             <a :href="link.url" class="upperText">{{link.text}}</a>
             </li>
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
    .dc-header {

        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0px 70px;

        .head-logo img {

            width: 60%;
            padding: 10px 0px;
            
        }

        .nav {

            ul {

                display: flex;
                list-style: none;
                font-size: 0.6em;
                
                li {



                    padding: 0px 10px;
                    border-bottom: 5px solid;


                      .active {

                        border-bottom:  black 5px solid;
                    }
                    a {
                    text-decoration: none;
                    color: black;
                    line-height: 90px;
                    padding: 10px 0px;
                    


                }

                }
            }
        }
    }
</style>