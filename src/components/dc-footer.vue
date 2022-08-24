<template>
    <div class="dc-footer">
      myfooter
        <div class="footer-nav">
            <div class="nav-links">
                <ul v-for="(link, index) in dccomics" :key="index">
                    <li><a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a></li>
                </ul>

                <ul v-for="(link, index) in shop" :key="index">
                    <li><a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a></li>
                </ul>

                <ul v-for="(link, index) in dc" :key="index">
                    <li><a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a></li>
                </ul>

                <ul v-for="(link, index) in sites" :key="index">
                    <li><a :href="link.url" :class ="link.active = true?'active':''" class="upperText">{{link.text}}</a></li>
                </ul>

            </div>
        </div>
        <div class="footer-signup">
            <button>Sign-Up Now!</button>
            <a href="#">follow us</a>
                <ul v-for="(link, index) in socialfoot" :key="index">
                    <li><a :href="link.url">{{link.img}}<img src="link.img" alt=""></a></li>
                </ul>
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
                    active: false
                },

                {
                    text: 'Shop DC collectbles',
                    url: '#',
                    active: true
                },

                
            ],
       
        

            dc: [
                {
                    text: 'Terms of Use',
                    url: '#',
                    active: false
                },

                {
                    text: 'Privacy policy',
                    url: '#',
                    active: true
                },

                {
                    text: 'Ad Choice',
                    url: '#',
                    active: true
                },

                {
                    text: 'Adversting',
                    url: '#',
                    active: true
                },

                {
                    text: 'Jobs',
                    url: '#',
                    active: true
                },

                {
                    text: 'Subscriptions',
                    url: '#',
                    active: true
                },

                {
                    text: 'Talent Workshops',
                    url: '#',
                    active: true
                },

                {
                    text: 'CPSC Certificates',
                    url: '#',
                    active: true
                },

                {
                    text: 'Ratings',
                    url: '#',
                    active: true
                },

                {
                    text: 'Shop Help',
                    url: '#',
                    active: true
                },

                {
                    text: 'Contact us',
                    url: '#',
                    active: true
                },
            ],

            sites: [
                {
                    text: 'DC',
                    url: '#',
                    active: false
                },

                {
                    text: 'MAD Magazine',
                    url: '#',
                    active: true
                },

                {
                    text: 'DC kids',
                    url: '#',
                    active: true
                },

                {
                    text: 'DC Universe',
                    url: '#',
                    active: true
                },

                {
                    
                    text: 'DC Power Visa',
                    url: '#',
                    active: true
                },

            ],

           socialfoot: [
                {
                    img: '../assets/img/footer-facebook',
                    url: '#',
                    active: false
                },

                {
                    img: '../assets/img/footer-periscope',
                    url: '#',
                    active: true
                },

                {
                    img: '../assets/img/footer-pinterest',
                    url: '#',
                    active: true
                },

                {
                    img: '../assets/img/footer-twitter',
                    url: '#',
                    active: true
                },

                {
                    
                    img: '../assets/img/footer-youtube',
                    url: '#',
                    active: true
                },

            ],
        

        
                
        }
            
    }
}
</script>

<style>

.footer-nav {

    background-image: url('../assets/img/footer-bg.jpg');
    height: 500px;
    position: relative;
    background-repeat: no-repeat;
}

.nav-links {

    display: flex;
    flex-wrap: wrap;
}
</style>