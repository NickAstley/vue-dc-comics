<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="row py-5">
                        <div class="col">
                            <h5 class="mb-3">{{ footerCategories[0].title }}</h5>
                            <ul class="list-unstyled">
                                <li v-for="(link, i) in footerCategories[0].links" :key="i">
                                    <a href="#">
                                        {{ link }}
                                    </a>
                                </li>
                            </ul>
                            <h5 class="mb-3">{{ footerCategories[1].title }}</h5>
                            <ul class="list-unstyled">
                                <li v-for="(link, i) in footerCategories[1].links" :key="i">
                                    <a href="#">
                                        {{ link }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="col">
                            <h5 class="mb-3">{{ footerCategories[2].title }}</h5>
                            <ul class="list-unstyled">
                                <li v-for="(link, i) in footerCategories[2].links" :key="i">
                                    <a href="#">
                                        {{ link }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div class="col">
                            <h5 class="mb-3">{{ footerCategories[3].title }}</h5>
                            <ul class="list-unstyled">
                                <li v-for="(link, i) in footerCategories[3].links" :key="i">
                                    <a href="#">
                                        {{ link }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col dc-bg">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        data () {
            return {
                footerCategories: [
                    {
                        title: "DC Comics",
                        links: [
                            "Characters",
                            "Comics",
                            "Movies",
                            "TV",
                            "Games",
                            "Videos",
                            "News"
                        ]
                    },
                    {
                        title: "Shop",
                        links: [
                            "Shop DC",
                            "Shop DC Collectibles"
                        ]
                    },
                    {
                        title: "DC",
                        links: [
                            "Terms Of Use",
                            "Privacy policy (New)",
                            "Ad Choices",
                            "Advertising",
                            "Jobs",
                            "Subscriptions",
                            "Talent Workshops",
                            "CPSC Certificates",
                            "Ratings",
                            "Shop Help",
                            "Contact Us"
                        ]
                    },
                    {
                        title: "Sites",
                        links: [
                            "DC",
                            "MAD Magazine",
                            "DC Kids",
                            "DC Universe",
                            "DC Power Visa"
                        ]
                    }
                ]
            }
        }
    }
</script>

<style lang="scss">
    footer {
        background-image: url("../assets/img/footer-bg.jpg");
        background-position: top center;
        background-repeat: no-repeat;
        background-size: cover;

        h5 {
            color: white;
            text-transform: uppercase;
        }

        li {
            a {
                color: #7C7979;
                text-decoration: none;
                font-size: 0.9rem;
            }
        }

        .dc-bg {
            background-image: url("../assets/img/dc-logo-bg.png");
            background-position: center;
            background-repeat: no-repeat;
        }
    }
</style>