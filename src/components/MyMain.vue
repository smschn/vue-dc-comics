<template>
    <main>
        <div class="containerWidth">
            --> content goes here
        </div>
    </main>
</template>

<script>
export default {
    name: 'MyMain'
}
</script>

<style lang="scss">

@import '../styles/container_width.scss';

main {
    background-color: #1c1c1c;
    height: 300px;
    width: 100%;
    color: white;

    div {
       height: 100%;
    }
}

</style>