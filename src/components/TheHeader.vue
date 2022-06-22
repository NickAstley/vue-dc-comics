<template>
    <header>
        <nav class="navbar navbar-expand-lg">
            <div class="container">
                <a class="navbar-brand" href="#">
                    <img src="../assets/img/dc-logo.png" alt="Logo DC">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse justify-content-end" id="navbarSupportedContent">
                    <ul class="navbar-nav mb-2 mb-lg-0">
                        <li class="nav-item text-uppercase" v-for="link in navLinks" :key="link">
                            <a class="nav-link px-3" :class="link === `Comics` ? `active` : ``" aria-current="page" href="#">{{ link }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
    export default {
        data () {
            return {
                navLinks: [
                    "Characters",
                    "Comics",
                    "Movies",
                    "TV",
                    "Games",
                    "Collectibles",
                    "Videos",
                    "Fans",
                    "News",
                    "Shop"
                ]
            }
        }
    }
</script>

<style lang="scss">
    @import "../assets/scss/variables";

    li.nav-item {
        font-weight: 600;

        a {
            color: inherit;

            &.active {
                position: relative;
                color: $bs-primary;

                &::after {
                    content: "";
                    width: 70%;
                    height: 0.5rem;
                    background: $bs-primary;
                    position: absolute;
                    bottom: -2.75rem;
                    left: 15%;
                    right: 15%;
                }
            }
        }
    }
</style>