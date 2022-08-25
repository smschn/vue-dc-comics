<template>
    <main>
        <div class="containerWidth">
            <div>prova</div>
            <div>prova</div>
            <div>prova</div>
            <div>prova</div>
            <div>prova</div>
            <div>prova</div>
            <div>prova</div>
            <div>prova</div>
            <div>prova</div>

        </div>
        <div class="button">LOAD MORE</div>
    </main>
</template>

<script>
export default {
    name: 'MyMain'
}
</script>

<style lang="scss">

@import '../styles/container_width.scss';
@import '../styles/variables.scss';
@import '../styles/mixins.scss';

main {
    background-color: #1c1c1c;
    width: 100%;
    height: 800px; // da togliere alla fine?
    color: white;

    .button {
        @include button();
        width: 150px;
        position: relative;
        left: 50%; // per centrarlo su asse X
        transform: translateX(-50%); // per centrarlo su asse X
    }
}

</style>