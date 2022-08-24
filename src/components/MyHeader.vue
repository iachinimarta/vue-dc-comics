<template>
    <header>
        <div class="logo">
            <a href="#">Logo</a>
        </div>

        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a href="link.url">{{link.text}}</a>
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

<style>

</style>