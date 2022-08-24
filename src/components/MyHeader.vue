<template>
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="Logo">
        </div>
        <nav>
            <ul>
                <li v-for='(link, index) in links' v-bind:key=index>
                    <a v-bind:href='link.url'>{{link.text}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    active: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    active: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    active: false
                },
                {
                    text: 'TV',
                    url: '#',
                    active: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    active: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    active: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    active: false
                }
            ]
        }
    }
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

        a {
            text-decoration: none;
            font-weight: bold;
            color: black;

            &:hover {
            color: #0282f9;
            cursor: pointer;
            }
        }
    }

}
</style>