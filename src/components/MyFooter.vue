<template>
    <footer>
        <div class="f_top">
            <div class="ft_container">
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
            <p>prova</p>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'MyFooter'
}
</script>

<style lang="scss">
footer {
    color: white;

    .f_top {
        background-image: url('../assets/img/footer-bg.jpg');

        .ft_container {
            width: 80%;
            margin: auto;
            height: 400px;
            display: flex;
            justify-content: space-between;

            .ft_menu {
                display: flex;

                li {
                    list-style: none;
                    color: grey;
                }
            }

            .ft_logobg {
                overflow: hidden;
            }
            }
    }

    .f_bottom {
        color: grey;
    }
}
</style>