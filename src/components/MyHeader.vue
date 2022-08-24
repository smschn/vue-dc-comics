<template>
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="Logo">
        </div>
        <nav>
            <ul>
                <li>CHARACTERS</li>
                <li>COMICS</li>
                <li>MOVIES</li>
                <li>TV</li>
                <li>GAMES</li>
                <li>COLLECTIBLES</li>
                <li>VIDEOS</li>
                <li>FANS</li>
                <li>NEWS</li>
                <li>SHOP</li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'MyHeader'
}
</script>

<style lang="scss">
header {
    width: 80%;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    li {
        list-style: none;
        display: inline-block;
        padding: 0px 10px;
        font-weight: bold;

        &:hover {
            color: #0282f9;
            cursor: pointer;
        }
    }
}
</style>