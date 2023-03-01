<template>
    <div id="bg-color-blue">
        <div class="container">
            <ul class="menu">
                <li class="menu-item">
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
                </li>
            </ul>
        </div>
    </div>

    <div class="bg-dc">
        <div class="container">
            <div class="list">

                <div class="col">
                    <ul>
                        <h1>Title</h1>
                        
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                    </ul>
                    
                    <ul>
                        <h1>Title</h1>
                        
                        <li>text</li>
                        <li>text</li>
                    </ul>
                </div>
                
                <div class="col">
                    <ul>
                        <h1>Title</h1>
                        
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                    </ul>
                </div>

                <div class="col">
                    <ul>
                        <h1>Title</h1>
                        
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
                        <li>text</li>
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

</script>

<style lang="scss">
    #bg-color-blue{
        background-color: #0282F9;
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
        background-color: #303030;
        padding: 40px 0;
        position: relative;
        top: -120px;
        .footer-social{
            flex-direction: row;
            justify-content: space-between;
            align-items: center;

            .sign-btn{
                padding: 20px;
                border: 3px solid #0282F9;
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
                    color: #0282F9;
                    text-transform: uppercase;
                    font-size: 30px;
                    padding-right: 20px;
                }
            }
        }

    }
</style>