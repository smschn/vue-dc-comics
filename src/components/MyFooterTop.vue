<template>
  <section id="footer_top">
    <div class="containerWidth">
        <div class="card" v-for="(card, index) in cards" v-bind:key="index">
            <img v-bind:src="card.imgSrc" v-bind:alt="card.altText">
            <div>{{card.text}}</div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'MyFooterTop',
    data() {
        return {
            cards: [
                {
                    imgSrc: '../assets/img/buy-comics-digital-comics.png',
                    altText: 'Ditigal Comics',
                    text: 'DIGITAL COMICS'
                },
                {
                    imgSrc: '../assets/img/buy-comics-merchandise.png',
                    altText: 'Dc Merchandise',
                    text: 'DC MERCHANDISE'
                },
                {
                    imgSrc: '../assets/img/buy-comics-subscriptions.png',
                    altText: 'Subscription',
                    text: 'SUBSCRIPTION'
                },
                {
                    imgSrc: '../assets/img/buy-comics-shop-locator.png',
                    altText: 'Comic Shop Locator',
                    text: 'COMIC SHOP LOCATOR'
                },
                {
                    imgSrc: '../assets/img/buy-dc-power-visa.svg',
                    altText: 'DC Power Visa',
                    text: 'DC POWER VISA'
                }
            ]
        }
    }
}
</script>

<style lang="scss">

@import '../styles/container_width.scss';
@import '../styles/variables.scss';

#footer_top {
    background-color: $blueDC;

    .containerWidth {
        padding: 40px;
        margin: auto;
        display: flex;
        justify-content: space-between;

        .card {
            flex-basis: calc(100% / 5);
        }
    }
}

</style>