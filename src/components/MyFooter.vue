<template>
    <footer>
        <div class="f_top">
            <div class="ft_container containerWidth">
                <div class="ft_menu">
                    <nav>
                        <h4>DC COMICS</h4>
                        <ul> <!-- creo dinamicamente il menu 'dc comics' -->
                            <li v-for="(link, index) in links_dcComics" v-bind:key="index"><a v-bind:href="link.url">{{link.text}}</a></li>
                        </ul>
                        <h4>SHOP</h4>
                        <ul> <!-- creo dinamicamente il menu 'shop' -->
                            <li v-for="(link, index) in links_shop" v-bind:key="index"><a v-bind:href="link.url">{{link.text}}</a></li>
                        </ul>
                    </nav>
                    <nav>
                        <h4>DC</h4>
                        <ul> <!-- creo dinamicamente il menu 'dc' -->
                            <li v-for="(link, index) in links_dc" v-bind:key="index"><a v-bind:href="link.url">{{link.text}}</a></li>
                        </ul>
                    </nav>
                    <nav>
                        <h4>SITES</h4>
                        <ul> <!-- creo dinamicamente il menu 'sites' -->
                            <li v-for="(link, index) in links_sites" v-bind:key="index"><a v-bind:href="link.url">{{link.text}}</a></li>
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
                    <li>FOLLOW US</li> <!-- creo dinamicamente le immagini social -->
                    <li v-for="(social, index) in socials" v-bind:key="index"><img v-bind:src="require(`../assets/img/footer-${social.imgSrc}`)" v-bind:alt="social.text"></li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>

export default {

    name: 'MyFooter',

    data() {
        return {
            
            // creo oggetti per creare dinamicamente le voci del menu

            links_dcComics: [ 
                {
                    text: 'Characters',
                    url: 'https://www.google.com'
                },
                {
                    text: 'Comics',
                    url: '#'
                },
                {
                    text: 'Movies',
                    url: '#'
                },
                {
                    text: 'TV',
                    url: '#'
                },
                {
                    text: 'Games',
                    url: '#'
                },
                {
                    text: 'Videos',
                    url: '#'
                },
                {
                    text: 'News',
                    url: '#'
                }
            ],

            links_shop: [
                {
                    text: 'Shop DC',
                    url: '#'
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#'
                }
            ],

            links_dc: [
                {
                    text: 'Terms Of Use',
                    url: '#'
                },
                {
                    text: 'Privacy Policy',
                    url: '#'
                },
                {
                    text: 'Ad Choices',
                    url: '#'
                },
                {
                    text: 'Jobs',
                    url: '#'
                },
                {
                    text: 'Subscriptions',
                    url: '#'
                },
                {
                    text: 'Talent Workshops',
                    url: '#'
                },
                {
                    text: 'CPSC Certificates',
                    url: '#'
                },
                {
                    text: 'Ratings',
                    url: '#'
                },
                {
                    text: 'Shop Help',
                    url: '#'
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#'
                },
                {
                    text: 'Contact Us',
                    url: '#'
                }
            ],

            links_sites: [
                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'MAD Magazine',
                    url: '#'
                },
                {
                    text: 'DC Kids',
                    url: '#'
                },
                {
                    text: 'DC Universe',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    url: '#'
                },
            ],

            socials: [
                {
                    imgSrc: 'facebook.png',
                    text: 'Facebook'
                },
                {
                    imgSrc: 'twitter.png',
                    text: 'Twitter'
                },
                {
                    imgSrc: 'youtube.png',
                    text: 'Youtube'
                },
                {
                    imgSrc: 'pinterest.png',
                    text: 'Pinterest'
                },
                {
                    imgSrc: 'periscope.png',
                    text: 'Periscope'
                }
            ]
        }
    }
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
                    padding: 5px 0px;

                    a {
                        text-decoration: none;
                        color: grey;

                        &:hover {
                            color: rgb(175, 175, 175);
                        }
                    }
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