<template>
    <div class="element-container">
        <div class="title">{{title}}</div>
        <ul>
            <li class="title-li" v-for="(url, index) in urls" :key="index">
                <a href="url.url">
                    {{url.text}}
                </a>
            </li>
        </ul>
    </div>
  
</template>

<script>
    export default {
        name: 'FooterMenu',
        props: {
            title: String,
            urls: Array,
            color: String
        }
    }
</script>

<style lang="scss">
    .element-container {
        margin: 0 20px;

        .title {
            margin-bottom: 10px;
        }

        a {
            color: lightgrey;
        }
    }

</style>