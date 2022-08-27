<template>
    <header>
        <div class="container90">
            <a href="#">
                <img src="../assets/img/dc-logo.png" alt="">
            </a>

            <nav>
                <ul>
                    <li v-for="(link, index) in links" :key="index" :class="link.active == true? 'active' : ''">
                        <a href="link.url">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
        
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

<style scoped lang="scss">

    header {
        background-color: #FFFFFF;
        padding: 10px;
        height: 90px;
        position: fixed;
        top: 0;
        left: 0;
        z-index: 999;
        width: 100%;

        .container90 {
            display: flex;
            justify-content: space-between;
            align-items: center;

            img {
                width: 100%;
                height: 70px;
            }

            ul {
                display: flex;     
                
                li {
                    margin: 0 5px;
                    
                    a {
                        color: black;
                        font-weight: bold;
                    }
                }
            }
        }       
    }

</style>