<template>
    <div class="bg-primary">
        <div class="container">
            <div class="row py-5 align-items-center">
                <div v-for="link in blueBannerLinks" :key="link.text" class="col">
                    <a href="#" class="row align-items-center">
                        <img class="col-auto" :src="require(`../assets/img/buy-${link.imgSrc}`)" :alt="`Immagine ` + link.text">
                        <span class="col text-white text-uppercase">{{ link.text }}</span>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                blueBannerLinks: [
                    {
                        text: "Digital Comics",
                        imgSrc: "comics-digital-comics.png"
                    },
                    {
                        text: "DC Merchandise",
                        imgSrc: "comics-merchandise.png"
                    },
                    {
                        text: "Subscription",
                        imgSrc: "comics-subscriptions.png"
                    },
                    {
                        text: "Comic Shop Locator",
                        imgSrc: "comics-shop-locator.png"
                    },
                    {
                        text: "DC power Visa",
                        imgSrc: "dc-power-visa.svg"
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    img {
        transform: scale(0.7);
        max-width: 120px;
        max-height: 100px;
    }
</style>