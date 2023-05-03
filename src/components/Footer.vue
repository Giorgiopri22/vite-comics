<script>

export default {
    name:"Footer",
    data() {
        return {
            arraylinkFooter: [
                {
                    title: 'Dc Comics',
                    link: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Videos',
                        'News'
                    ],
                    shop: [{
                        title: 'Shop',
                        link: [
                            'Shop DC',
                            'Shop DC Collectibles'
                        ]
                    }]
                },
                {
                    title: 'Dc',
                    link: [
                        'Terms Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us'
                    ]
                },
                {
                    title: 'Sites',
                    link: [
                        'DC',
                        'MAD Magazine',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ]
                },
            ],

            arrayIcon: [
                './src/assets/img/footer-youtube.png',
                './src/assets/img/footer-twitter.png',
                './src/assets/img/footer-pinterest.png',
                './src/assets/img/footer-periscope.png',
                './src/assets/img/footer-facebook.png'
            ]
    
            
        }
    }
}

</script>

<template>

    <footer>
        <div class="section-link">
            <div class="container">
                <div class="link">
                    <ul v-for="objectLink in arraylinkFooter">
                        <h3 class="title">
                            {{ objectLink.title }}
                        </h3>
                        <li class="text"
                        v-for="link in objectLink.link">
                            {{ link }}
                        </li>
                        <ul class="shopUl"
                        v-for="shop in objectLink.shop">
                            <h3 class="title">
                                {{ shop.title }}
                            </h3>
                            <li class="text"
                            v-for="linkShop in shop.link">
                                {{ linkShop }}
                            </li>
                        </ul>
                    </ul>
                </div>
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="logo-big">
                </div>
            </div>
        </div>
        <div class="section-sign-up">
            <div class="container">
                <div class="row">
                    <div class="col-button">
                        Sign-up Now!
                    </div>
                    <div class="col-icon">
                        <div class="text">
                            Follow us
                        </div>
                        <ul class="icon-list">
                            <li v-for="icon in arrayIcon">
                                <img :src="icon" alt="icon">
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>

<style lang="scss" scoped>



</style>