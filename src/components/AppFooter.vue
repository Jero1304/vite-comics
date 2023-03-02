<template>
    <div id="bg-color-blue">
        <div class="container">
            <ul class="menu">
                <!-- <li class="menu-item">
                    <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                    <p>digital comics</p>
                </li>
                <li class="menu-item">
                    <img src="../../public/img/buy-comics-merchandise.png" alt="">
                    <p>dc merchandise</p>
                </li>
                <li class="menu-item">
                    <img src="../../public/img/buy-comics-subscriptions.png" alt="">
                    <p>subscription</p>
                </li>
                <li class="menu-item">
                    <img src="../../public/img/buy-comics-shop-locator.png" alt="">
                    <p>comic shop locator</p>
                </li>
                <li class="menu-item">
                    <img src="../../public/img/buy-dc-power-visa.svg" alt="">
                    <p>dc power visa</p>
                </li> -->

                <FooterShop v-for="(icon, i) in shop.icons"
                :key="i" :icon="icon" :text="shop.texts[i]"/>
            </ul>
        </div>
    </div>

    <div class="bg-dc">
        <div class="container">
            <div class="list">

                <div class="col">
                    <ul>
                        <h1>{{ menu1.title }}</h1>
                        <FooterMenu 
                        v-for="(link, i) in menu1.links" 
                        :key="i" 
                        :title="menu1.title" 
                        :link="link"/>                                                
                    </ul>
                    
                    <ul>
                        <h1>{{ menu2.title }}</h1>
                        <FooterMenu 
                        v-for="(link, i) in menu2.links" 
                        :key="i" 
                        :title="menu2.title" 
                        :link="link"/>                                                              
                    </ul>
                </div>
                
                <div class="col">
                    <ul>
                        <h1>{{ menu3.title }}</h1>
                        <FooterMenu 
                        v-for="(link, i) in menu3.links" 
                        :key="i" 
                        :title="menu3.title" 
                        :link="link"/> 
                    </ul>
                </div>

                <div class="col">
                    <ul>
                        <h1>{{ menu4.title }}</h1>
                        <FooterMenu 
                        v-for="(link, i) in menu4.links" 
                        :key="i" 
                        :title="menu4.title" 
                        :link="link"/> 
                    </ul>
                </div>

                <div class="dc-logo">
                    <img src="../../public/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </div>

    <div class="social">
        <div class="container">
            <div class="row footer-social">
                <a href="#" class="sign-btn">
                    Sign-up Now!
                </a>

                <div class="social-contact">
                    <h1>follow us</h1>
                    <img src="../../public/img/footer-facebook.png" alt="">
                    <img src="../../public/img/footer-twitter.png" alt="">
                    <img src="../../public/img/footer-youtube.png" alt="">
                    <img src="../../public/img/footer-pinterest.png" alt="">
                    <img src="../../public/img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </div>
    
</template>

<script>
    import FooterMenu from "./FooterMenu.vue";
    import FooterShop from "./FooterShop.vue";
    export default{
        components:{
            FooterMenu,
            FooterShop
        },
        data(){
            return{
                menu1:{
                    title:'dc comics',
                    links:[
                        'charter',
                        'comics',
                        'TV',
                        'games',
                        'videos',
                        'news'
                    ]
                },
                menu2:{
                    title:'Shop',
                    links:[
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                },    
                menu3:{
                    title:'dc',
                    links:[
                        'Terms of use',
                        'privacy policy (new)',
                        'jobs',
                        'subscription',
                        'Talent Workshop',
                        'CPSC certificates',
                        'Ratings',
                        'shop help',
                        'Contact use',
                    ]
                },
                menu4:{
                    title:'sites',
                    links:[
                        'dc',
                        'MAD megazine',
                        'DC kids',
                        'DC universe',
                        'dc power Visa',
                    ]
                },

                shop:{
                    icons:[
                        '../../public/img/buy-comics-digital-comics.png',
                        '../../public/img/buy-comics-merchandise.png',
                        '../../public/img/buy-comics-subscriptions.png',
                        '../../public/img/buy-comics-shop-locator.png',
                        '../../public/img/buy-dc-power-visa.svg'
                    ],
                    texts:[
                        'digital comics',
                        'dc merchandise',
                        'subscription',
                        'comic shop locator',
                        'dc power visa'
                    ]
                }                
            }
        }
    }
</script>

<style lang="scss">
@use '../style/patrials/variables' as*;
    #bg-color-blue{
        background-color: $blue;
    }
    .menu{
            display: flex;
            justify-content: center;
            justify-content: space-between;
            padding: 40px 0;
            .menu-item{
                display: flex;
                align-items: center;
                justify-content: center;
                padding: 10px;
                font-size: 15px;
                text-transform: uppercase;
                color: white;
                img{
                    padding: 0 10px;
                    max-width: 70px;
                }
            }
        }
    .bg-dc{
        background-image: url('../../public/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;

        .list{
            display: flex;
            flex-direction: row;
            
            .col{
                color: white;
                padding: 40px 50px 0 0 ;
    
                ul{
                    padding-bottom: 30px;
                    h1{
                    padding-bottom: 15px;
                    font-size: 30px;
                    text-transform: uppercase;
                    }
                    li{
                        padding-bottom: 7px;
                        color: lightgrey;
                        text-transform: capitalize
                    }
                }
            }
            .dc-logo{
                display: flex;
                justify-content: end;
                flex-grow: 1;
                position: relative;
                top:-70px;
            }
        }
    }

    .social{
        background-color: $black;
        padding: 40px 0;
        position: relative;
        top: -120px;
        .footer-social{
            flex-direction: row;
            justify-content: space-between;
            align-items: center;

            .sign-btn{
                padding: 20px;
                border: 3px solid $blue;
                color: white;
                text-transform: uppercase;
                font-size: 20px;
                font-weight: bold;
            }

            .social-contact{
                display: flex;
                align-items: center;

                img{
                    padding: 0 10px;
                }
                h1{
                    color: $blue;
                    text-transform: uppercase;
                    font-size: 30px;
                    padding-right: 20px;
                }
            }
        }

    }
</style>