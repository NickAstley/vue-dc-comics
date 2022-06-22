<template>
  <div id="app">
    <TheHeader/>
    <main>
      <div class="container">
        <h1>--&gt; Content goes here &lt;--</h1>
      </div>
    </main>
    <BannerBlue/>
    <TheFooter/>
    <BannerSignUp/>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader"
import BannerBlue from "./components/BannerBlue"
import TheFooter from "./components/TheFooter"
import BannerSignUp from "./components/BannerSignUp"

export default {
  name: 'App',
  components: {
    TheHeader,
    BannerBlue,
    TheFooter,
    BannerSignUp
  }
}
</script>