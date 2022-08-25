<template>
    <footer>
        <div class="wrapper-top">
            <div class="container">
                <ul>
                    <li v-for="(linkfooter, indice) in linkfoot" :key="indice">
                        <div class="wrapper-link">
                            <div class="img_link">
                                <img :src="linkfooter.img" alt="">
                            </div>
                            <a :href="linkfooter.direzione">{{linkfooter.nome}}</a>
                        </div>
                    </li>
                </ul>
            </div>
        </div>

        <div class="wrapper-mid">
            <div class="container">
                <div class="cols">
                    <div class="col">
                        <div class="cont-col">
                            <h2>DC COMICS</h2>
                            <ul>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Comics</li>
                            </ul>

                            <h2>SHOP</h2>
                            <ul>
                                <li>Shop DC</li>
                                <li>ShopDC Collectibles</li>
                            </ul>
                        </div>

                        <div class="cont-col">
                            <h2>DC</h2>
                            <ul>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Comics</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Comics</li>
                            </ul>
                        </div>

                        <div class="cont-col">
                            <h2>SITES</h2>
                            <ul>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Comics</li>
                                <li>Movies</li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-img">
                        <img src="@/assets/img/dc-logo-bg.png">
                    </div>
                </div>
            </div>
        </div>


        <div class="wrapper-bot">
            <div class="container">
                <div class="wrapper-footer-bot">
                    <button class="btn">SIGN-UP NOW!</button>
                    <div class="social">
                        <h2>FOLLOW AS</h2>
                        <img v-for="(social, indice) in social" :key="indice" :src="social.url" :alt="social.nome">
                    </div>
                </div>                   
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    nome: 'MyFooter',
    data(){
        return{
            linkfoot:   [
                            {
                                nome: 'DIGITAL COMICS',
                                direzione: '#',
                                img: require ('@/assets/img/buy-comics-digital-comics.png')
                            },
                            {
                                nome: 'DC MERCHANDISE',
                                direzione: '#',
                                img: require ('@/assets/img/buy-comics-merchandise.png')
                            },
                            {
                                nome: 'SUBSCRIPTION',
                                direzione: '#',
                                img: require ('@/assets/img/buy-comics-subscriptions.png')
                            },
                            {
                                nome: 'COMIC SHOP LOCATOR',
                                direzione: '#',
                                img: require ('@/assets/img/buy-comics-shop-locator.png')
                            },
                            {
                                nome: 'DC POWER VISA',
                                direzione: '#',
                                img: require ('@/assets/img/buy-dc-power-visa.svg')
                            },
                        ],
            social:     [
                            {
                                url: require ('@/assets/img/footer-facebook.png') ,
                                nome: 'facebook'
                            },
                            {
                                url: require ('@/assets/img/footer-twitter.png'),
                                nome: 'twitter'
                            },
                            {
                                url: require ('@/assets/img/footer-youtube.png'),
                                nome: 'youtube'
                            },
                            {
                                url: require ('@/assets/img/footer-pinterest.png'),
                                nome: 'pinterest'
                            },
                            {
                                url: require ('@/assets/img/footer-periscope.png'),
                                nome: 'periscope'
                            },
                        ]
        }
    }
}
</script>

<style lang="scss">
    @import '../style/vars.scss';
    @import '../style/mixin.scss';
    footer{
        height: calc(100% - 250px);
        background-image: url('../assets/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        .wrapper-top{
            height: 130px;
            background-color: $brand-color;
            @include spaziatura('spalbetween');
            ul{
                display: flex;
                align-items: center;
                justify-content: space-between;
                height: 100%;
                padding: 10px;
                li{
                    list-style: none;
                    
                    .wrapper-link{
                            display: flex;
                            align-items: center;
                            justify-content: center;
                        .img_link{
                            width: 40px;
                            margin-right: 10px;
                            
                            img{
                                width: 100%;
                                object-fit: cover;
                                                             
                            }
                        }
                        a{
                            line-height: 100%;
                            text-decoration: none;
                            color: white;
                        }
                    }
                }
            }
        }
        .wrapper-mid{
            height: calc(100% - 230px);
            .cols{
                display: flex;
                justify-content: space-between;
                height: 100%;
                .col{
                    width: 50%;
                    height: 100%;
                    display: flex;
                    padding-top: 50px;
                    .cont-col{
                        margin-right: 40px;
                        height: 100%;
                        h2{
                            color: white;
                            margin: 10px 0;
                        }
    
                        li{
                            list-style: none;
                            font-size: 17px;
                            color: gray;
                            line-height: 25px;
                        }
                    }
                }
                .col-img{
                    width: 38%;
                    img{
                        width: 100%;
                        height: 100%;
                        object-fit: cover;
                    }
                }
            }
        }
        .wrapper-bot{
            @include spaziatura('spalbetween');
            z-index: 999;
            height: 100px;
            background-color: #303030;
            .wrapper-footer-bot{
                height: 100%;
                display: flex;
                justify-content: space-between;
                align-items: center;
                .btn{
                    
                    padding: 10px;
                    font-size: 18px;
                    border: 1px solid ;
                    color: $brand-color;
                    background-color: #303030;
                }
                .social{
                    display: flex;
                    align-items: center;
                    color: gray;
                    img{
                        margin-left: 15px;
                    }
                }
            }
        }
    }
</style>