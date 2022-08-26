<template>
    <div class="dc-footer">
        <div class="footer-nav">
            <div class="nav-links">
                <ul>
                    <h3>DC COMICS</h3>
                    <li v-for="(link, index) in dccomics" :key="index">
                    <a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a>
                    </li>

                    <ul class="inner-ul">
                    <h3>SHOP</h3>
                    <li v-for="(link, index) in shop" :key="index">
                    <a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a>
                    </li>
                </ul>

                </ul>
                <ul>
                    <h3>DC</h3>
                    <li v-for="(link, index) in dc" :key="index">
                    <a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a>
                    </li>
                </ul>

                <ul>
                    <h3>SITES</h3>
                    <li v-for="(link, index) in sites" :key="index">
                    <a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a>
                    </li>
                </ul>

            </div>
            <div class="footer-bg-img">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
        <div class="footer-signup">
            <a href="#" class="button">Sign-Up Now!</a>
            <div class="social-icons">
                <a href="#">follow us</a>
                    <ul v-for="(link, index) in socialfoot" :key="index">
                        <li><a :href="link.url"><img :src="link.img" alt=""></a></li>
                    </ul>
            </div>
        </div>
    </div>
</template>

<script>

export default {
     name: 'DCfooter',
     data() {
        return { 

                dccomics: [
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
            ],
      

       

            shop: [
                {
                    text: 'Shop DC',
                    url: '#',
                   
                },

                {
                    text: 'Shop DC collectbles',
                    url: '#',
                  
                },

                
            ],
       
        

            dc: [
                {
                    text: 'Terms of Use',
                    url: '#',
                    
                },

                {
                    text: 'Privacy policy',
                    url: '#',
                   
                },

                {
                    text: 'Ad Choice',
                    url: '#',
                   
                },

                {
                    text: 'Adversting',
                    url: '#',
                  
                },

                {
                    text: 'Jobs',
                    url: '#',
                 
                },

                {
                    text: 'Subscriptions',
                    url: '#',
                   
                },

                {
                    text: 'Talent Workshops',
                    url: '#',
                  
                },

                {
                    text: 'CPSC Certificates',
                    url: '#',
                    
                },

                {
                    text: 'Ratings',
                    url: '#',
                   
                },

                {
                    text: 'Shop Help',
                    url: '#',
                   
                },

                {
                    text: 'Contact us',
                    url: '#',
                    
                },
            ],

            sites: [
                {
                    text: 'DC',
                    url: '#',
                   
                },

                {
                    text: 'MAD Magazine',
                    url: '#',
                   
                },

                {
                    text: 'DC kids',
                    url: '#',
                   
                },

                {
                    text: 'DC Universe',
                    url: '#',
                   
                },

                {
                    
                    text: 'DC Power Visa',
                    url: '#',
                  
                },

            ],

           socialfoot: [
                {
                    img: require('../assets/img/footer-facebook.png'),
                    url: '#',
                   
                },

                {
                    img: require('../assets/img/footer-periscope.png'),
                    url: '#',
                   
                },

                {
                    img: require('../assets/img/footer-pinterest.png'),
                    url: '#',

                },

                {
                    img: require('../assets/img/footer-twitter.png'),
                    url: '#',
                },

                {
                    
                    img: require('../assets/img/footer-youtube.png'),
                    url: '#',
                },

            ],
                
        }
            
    }
}
</script>

<style lang="scss">


.footer-nav {

    background-image: url('../assets/img/footer-bg.jpg');
    background-size: 100%;
    background-repeat: no-repeat;

    display: flex;
    justify-content: space-between;
    color:white;

   

      .footer-bg-img {
          
          height: 300px;
          overflow:hidden;
          padding-right: 100px;

          display: flex;
          align-items: center;
          

          img {

            width: 100%;
            height: 150%; 
            object-fit: contain;
            
           
      }
      }
    
}

.nav-links {
    display: flex;
    gap:20px;
    padding:20px;

    ul{

         .inner-ul h3 {

        margin-top: 10px;
    }

        li{
            list-style:none;
            

            a{
                text-decoration: none;
                color:rgb(161, 161, 161);
                font-size: 0.6em;
            }
        }
        
    }
}

.footer-signup {

    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px;
    background-color: #2A2A2A;

    a.button {

            border: 2px solid  #0075F7;
            text-decoration: none;
            text-transform: uppercase;
            padding: 10px;
            color: white;

        }

    .social-icons {

        display: flex;
        align-items: center;
        gap:20px;
        margin-right: 50px;

        a {

            color: #0075F7;
            text-decoration: none;
            text-transform: uppercase;

        }

        li {

            list-style:none;
        }
    }

}

</style>