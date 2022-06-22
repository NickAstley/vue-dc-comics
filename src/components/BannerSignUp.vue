<template>
    <div class="sign-up-banner">   
        <div class="container">
            <div class="row py-4 justify-space-between">
                <div class="col">
                    <button type="button" class="btn btn-outline-primary text-uppercase">Sign-up Now!</button>
                </div>
                <div class="col">
                    <div class="row align-items-center">
                        <span class="col-auto text-primary fw-bold text-uppercase">Follow us</span>
                        <div class="col-auto text-center" v-for="social in socialMediaLinks" :key="social.site">
                            <img :src="require(`../assets/img/footer-${social.imgSrc}.png`)" alt="social.site">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                socialMediaLinks: [
                    {
                        site: "Facebook",
                        imgSrc: "facebook"
                    },
                    {
                        site: "Twitter",
                        imgSrc: "twitter"
                    },
                    {
                        site: "YouTube",
                        imgSrc: "youtube"
                    },
                    {
                        site: "Periscope",
                        imgSrc: "periscope"
                    },
                    {
                        site: "Pinterest",
                        imgSrc: "pinterest"
                    }
                ]
            }
        }
    }
</script>

<style lang="scss">
    .sign-up-banner {
        background: #303030;

        .btn-outline-primary {
            border-radius: 0;
            color: white;
            border-width: 2px;
        }
    }
</style>