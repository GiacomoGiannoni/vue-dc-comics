<template>
    <footer>
        <div class="d-flex container footerup">
            <div class="footer-links">
                <h4>DC COMICS</h4>
                <ul>
                    <li>
                        <a href="#">Characters</a>
                    </li>
                    <li>
                        <a href="#">Comics</a>
                    </li>
                    <li>
                        <a href="#">Movies</a>
                    </li>
                    <li>
                        <a href="#">Tv</a>
                    </li>
                    <li>
                        <a href="#">Games</a>
                    </li>
                    <li>
                        <a href="#">Videos</a>
                    </li>
                    <li>
                        <a href="#">News</a>
                    </li>
                </ul>

                <h4>SHOP</h4>

                <ul>
                    <li>
                        <a href="#">Shop DC</a>
                    </li>
                    <li>
                        <a href="#">Shop DC Collectibles</a>
                    </li>
                </ul>
            </div>

            <div class="footer-links">
                <h4>DC</h4>
                <ul>
                    <li>
                        <a href="#">Terms Of Use</a>
                    </li>
                    <li>
                        <a href="#">Privacy policy (new)</a>
                    </li>
                    <li>
                        <a href="#">Ad Choices</a>
                    </li>
                    <li>
                        <a href="#">Advertising</a>
                    </li>
                    <li>
                        <a href="#">Jobs</a>
                    </li>
                    <li>
                        <a href="#">Subscriptions</a>
                    </li>
                    <li>
                        <a href="#">Talent Workshops</a>
                    </li>
                    <li>
                        <a href="#">CPSC Certificates</a>
                    </li>
                    <li>
                        <a href="#">Ratings</a>
                    </li>
                    <li>
                        <a href="#">Shop Help</a>
                    </li>
                    <li>
                        <a href="#">Contact US</a>
                    </li>
                </ul>
            </div>

            <div class="footer-links">
                <h4>Sites</h4>
                <ul>
                    <li>
                        <a href="#">DC</a>
                    </li>
                    <li>
                        <a href="#">MAD Magazine</a>
                    </li>
                    <li>
                        <a href="#">DC Kids</a>
                    </li>
                    <li>
                        <a href="#">DC Universe</a>
                    </li>
                    <li>
                        <a href="#">DC Power Visa</a>
                    </li>
                </ul>
            </div>
             <a href="#">
                <img src="@/assets/img/dc-logo-bg.png">
            </a>
        </div>
        <div class="d-flex container footerdown">
            <h4>SIGN-UP NOW!</h4>
            <ul>
                <li>
                    <a href="#">FOLLOW US</a>
                </li>
                <li>
                    <a href="#"><img src="@/assets/img/footer-facebook.png"></a>
                </li>
                <li>
                    <a href="#"><img src="@/assets/img/footer-twitter.png"></a>
                </li>
                <li>
                    <a href="#"><img src="@/assets/img/footer-youtube.png"></a>
                </li>
                <li>
                    <a href="#"><img src="@/assets/img/footer-pinterest.png"></a>
                </li>
                <li>
                    <a href="#"><img src="@/assets/img/footer-periscope.png"></a>
                </li>
            </ul>
        </div>
    </footer>
</template>

<script>
    export default {
        name: 'MyFooter',
    }
</script>

<style scoped lang="scss">
    .footerup {
        background-image: url('../assets/img/footer-bg.jpg');
        padding: 30px;
        text-align: center;
    }

    .footerdown {
        background-color: #303030;
    }
</style>