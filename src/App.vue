<template>
  <div id="app">
    <TheHeader/>
    <ComicsCards/>
    <BannerBlue/>
    <TheFooter/>
    <BannerSignUp/>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader"
import ComicsCards from "./components/ComicsCards"
import BannerBlue from "./components/BannerBlue"
import TheFooter from "./components/TheFooter"
import BannerSignUp from "./components/BannerSignUp"

export default {
  name: 'App',
  components: {
    TheHeader,
    ComicsCards,
    BannerBlue,
    TheFooter,
    BannerSignUp
  }
}
</script>