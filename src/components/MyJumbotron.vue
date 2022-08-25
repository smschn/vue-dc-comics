<template>
  <section id="jumbotron">
    <div class="series_box">
        CURRENT SERIES
    </div>
  </section>
</template>

<script>
export default {
    name: 'MyJumbotron'
}
</script>

<style lang='scss'>
@import '../styles/variables.scss';
@import '../styles/mixins.scss';

#jumbotron {
    background-image: url('../assets/img/jumbotron.jpg');
    background-size: cover;
    height: 350px;

    .series_box {
        @include button(); // uso un mixin per le regole comuni dei due bottoni presenti nel progetto
        width: 170px;
        position: relative;
        bottom: -330px;
        left: 10%;
    }
}
</style>