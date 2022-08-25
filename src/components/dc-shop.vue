<template>
  <div class="dc-shop">
      <ul>
            <li  v-for="(link, index) in links" :key="index">
                <img :src="link.img" alt="dc shop">   
                <a :href="link.url" class="upperText">{{link.text}}</a>
                
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
                    img: require('../assets/img/buy-comics-digital-comics.png'),
                    text: 'Digital Comics',
                    url: '#',
                    active: false
                },

                {
                    img: require('@/assets/img/buy-comics-merchandise.png'),
                    text: 'Dc merchandise',
                    url: '#',
                    active: true
                },

                {
                    img: require('@/assets/img/buy-comics-subscriptions.png'),
                    text: 'subscription',
                    url: '#',
                    active: false
                },
                {
                    img: require('@/assets/img/buy-comics-shop-locator.png'),
                    text: 'comic shop locator',
                    url: '#',
                    active: false
                },

                {
                    img: require('@/assets/img/buy-dc-power-visa.svg'),
                    text: 'dc power visa',
                    url: '#',
                    active: false
                },
            ]
        
        }
    }
}
</script>

<style scoped lang="scss">

.dc-shop {
    background-color: #0075F7;
    padding: 50px 20px;
    
    
    
    ul{
        display: flex;
        justify-content:center;
        align-items: center;
        list-style: none;
        
        
        li {

                width: 150px;
                display: flex;
                align-items: center;
                margin-left: 30px;

            img {

                width:30%;
                height: 50px;
            
                
                
            }

            a {

                margin-left: 10px;
                text-decoration: none;
                color:white;
                text-transform: uppercase;
                font-size: 10px;
            }
        }
    }
}

</style>