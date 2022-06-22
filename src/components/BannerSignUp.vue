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
                            <img :src="require(`../assets/img/${social.img_src}`)" alt="social.site">
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
                        img_src: "footer-facebook.png"
                    },
                    {
                        site: "Twitter",
                        img_src: "footer-twitter.png"
                    },
                    {
                        site: "YouTube",
                        img_src: "footer-youtube.png"
                    },
                    {
                        site: "Periscope",
                        img_src: "footer-periscope.png"
                    },
                    {
                        site: "Pinterest",
                        img_src: "footer-pinterest.png"
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