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
                <div class="collapse navbar-collapse" id="navbarSupportedContent">
                    <ul class="navbar-nav mb-2 mb-lg-0">
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Characters</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link active" aria-current="page" href="#">Comics</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Movies</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">TV</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Games</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Collectibles</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Videos</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Fans</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">News</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" aria-current="page" href="#">Shop</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>

<script>
    export default {

    }
</script>

<style lang="scss">
    .navbar-collapse {
        justify-content: center;

        li.nav-item {
            font-weight: 600;
            text-transform: uppercase;

            a {
                color: black;

                &.active {
                    color: #0C7CEC;
                    position: relative;

                    &::after {
                        content: "";
                        width: 70%;
                        height: 0.5rem;
                        background: #0C7CEC;
                        position: absolute;
                        bottom: -2.75rem;
                        left: 15%;
                        right: 15%;
                    }
                }
            }
        }
    }
</style>