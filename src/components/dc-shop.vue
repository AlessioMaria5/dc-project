<template>
  <div class="dc-shop">
      <ul v-for="(link, index) in links" :key="index">
            <li>
                <img :src="link.img" alt="DC shop">   
                <a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a>
            </li>
         </ul>
  </div>
</template>

<script>



export default {
     name: 'DCshop',
      data() {
        return {
            links: [
                {
                    img: '@/assets/img/buy-comics-digital-comics.png',
                    text: 'Digital Comics',
                    url: '#',
                    active: false
                },

                {
                    img: '@/assets/img/buy-comics-digital-comics.png',
                    text: 'Dc merchandise',
                    url: '#',
                    active: true
                },

                {
                    img: '@/assets/img/buy-comics-digital-comics.png',
                    text: 'subscription',
                    url: '#',
                    active: false
                },
                {
                    img: '@/assets/img/buy-comics-digital-comics.png',
                    text: 'comic shop locator',
                    url: '#',
                    active: false
                },

                {
                    img: '@/assets/img/buy-comics-digital-comics.png',
                    text: 'Games',
                    url: '#',
                    active: false
                },

                {
                    img: '@/assets/img/buy-comics-digital-comics.png',
                    text: 'Collectibles',
                    url: '#',
                    active: false
                },

                {
                    img: '@/assets/img/buy-comics-digital-comics.png',
                    text: 'dc power visa',
                    url: '#',
                    active: false
                },
            ]
        
        }
    }
}
</script>

<style>

</style>