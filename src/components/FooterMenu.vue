<template>
    <div class="element-container">
        <h4 class="title">{{title}}</h4>
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