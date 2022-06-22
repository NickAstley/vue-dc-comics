<template>
  <div id="app">
    <TheHeader/>
    <main>
      <div class="container">
        <h1>--&gt; Content goes here &lt;--</h1>
      </div>
    </main>
    <TheFooter/>
    <BannerSignUp/>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader"
import TheFooter from "./components/TheFooter"
import BannerSignUp from "./components/BannerSignUp"

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter,
    BannerSignUp
  }
}
</script>

<style lang="scss">
  @import url(../src/assets/scss/main.scss);
</style>