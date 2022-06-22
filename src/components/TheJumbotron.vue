<template>
    <div class="jumbotron" :style="clickedImgSrc ? `background-image: url(${clickedImgSrc})` : ``">
    </div>
</template>

<script>
    export default {
        props: {
            clickedImgSrc: String
        }
    }
</script>

<style lang="scss">
    .jumbotron {
        background-image: url("../assets/img/jumbotron.jpg");
        background-position: top center;
        background-size: cover;
        height: 400px;
    }
</style>