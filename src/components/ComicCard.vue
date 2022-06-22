<template>
    <div>
        <div class="comic-container text-white">
            <div class="comic-img-container mb-3">
                <img :src="cardImg" :alt="cardTitle">
            </div>
            <span class="text-uppercase">{{ cardTitle }}</span>
            <div class="hover-info p-3">
                <div>
                    Price: {{ cardPrice }}
                </div>
                <div>
                    Category: {{ cardType }}
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        props: {
            cardImg: String,
            cardTitle: String,
            cardPrice: String,
            cardType: String
        }
    }
</script>

<style lang="scss">
    .comic-container {
        position: relative;

        .comic-img-container {
            overflow: hidden;
            aspect-ratio: 1 / 1;
        }
    
        .hover-info {
            display: none;
        }

        &:hover {
            .hover-info {
                display: block;
                position: absolute;
                top: 0;
                bottom: 0;
                left: 0;
                right: 0;
                background-color: rgba(0, 0, 0, 0.5);
            }
        }
    }
</style>