<template>
    <footer>
        <div class="f_top">
            <div class="ft_container containerWidth">
                <div class="ft_menu">
                    <nav>
                        <h4>DC COMICS</h4>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h4>SHOP</h4>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </nav>
                    <nav>
                        <h4>DC</h4>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy Policy</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </nav>
                    <nav>
                        <h4>SITES</h4>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </nav>
                </div>
                <div class="ft_logobg">
                    <img src="../assets/img/dc-logo-bg.png" alt="Logo_bg">
                </div>
            </div>
        </div>
        <div class="f_bottom">
            <div class="fb_container containerWidth">
                <button>SIGN UP NOW!</button>
                <ul>
                    <li>FOLLOW US</li>
                    <li><img src="../assets/img/footer-facebook.png" alt="Facebook"></li>
                    <li><img src="../assets/img/footer-twitter.png" alt="Twitter"></li>
                    <li><img src="../assets/img/footer-youtube.png" alt="Youtube"></li>
                    <li><img src="../assets/img/footer-pinterest.png" alt="Pinterest"></li>
                    <li><img src="../assets/img/footer-periscope.png" alt="Periscope"></li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter'
}
</script>

<style lang="scss">

@import '../styles/container_width.scss';
@import '../styles/variables.scss';

footer {
    color: white;

    .f_top {
        background-image: url('../assets/img/footer-bg.jpg');

        .ft_container {
            height: 450px;
            display: flex;
            justify-content: space-between;
            overflow: hidden; // nascondo la parte del logo che fuoriesce dal contenitore

            .ft_menu {
                display: flex;
                padding: 50px 0px;

                nav {
                    margin: 0px 10px;
                }

                nav h4 {
                    font-size: 1.2rem;
                    padding-bottom: 15px;
                }

                nav:first-child ul {
                    color: red;
                    margin-bottom: 20px;
                }

                li {
                    list-style: none;
                    color: grey;
                    padding: 5px 0px;
                }
            }

            .ft_logobg {
                position: relative;
                top: -60px;
            }
        }
    }

    .f_bottom {
        background-color: $bgFooter1;


        .fb_container {
            display: flex;
            justify-content: space-between;
            padding: 30px 0px;

            button {
                border: 1px solid $blueDC;
                background-color: $bgFooter1;
                color: #fff;
                padding: 15px;
            }

            ul {
                display: flex;
                align-items: center;
            }

            ul li {
                display: inline-block;
                padding: 0px 10px;
            }

            ul li:first-child {
                color: $blueDC;
                font-weight: bold;
            }
        }
    }
}

</style>