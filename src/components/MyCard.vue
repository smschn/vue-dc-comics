<template>
<div>
    <div class="card_comics">
        <div class="img_container">
            <img v-bind:src="details.thumb" v-bind:alt="details.type">
        </div>
        <h6>{{details.series.toUpperCase()}}</h6>
    </div>
</div>
</template>

<script>
export default {
    name: 'MyCard',
    props: {
        details: Object
    }
}
</script>

<style lang='scss'>
@import '../styles/container_width.scss';
@import '../styles/variables.scss';
@import '../styles/general_rules.scss';


.card_comics {
    flex-basis: calc(100% / 6);
    margin: 10px;
    max-width: 150px;

    .img_container { // per creare l'immagine quadrata e non rettangolare
    width: 150px;
    height: 150px;
    overflow: hidden;

        img { // per mostrare tutta l'immagine, mantenendone l'aspect ratio
            max-width: 100%;

            &:hover {
                opacity: 0.5;
            }
        }
    }
    
    h6 {
        margin-top: 10px;
        color: grey;

        &:hover {
            color: rgb(175, 175, 175);
        }
    }
    
}

</style>