<template>
  <div id="app">
    <TheHeader/>
    <main>
      <div class="container">
        <h1>--&gt; Content goes here &lt;--</h1>
      </div>
    </main>
    <TheFooter/>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader"
import TheFooter from "./components/TheFooter"

export default {
  name: 'App',
  components: {
    TheHeader,
    TheFooter
  }
}
</script>

<style lang="scss" scoped>
  @import url(../src/assets/scss/general.scss);
</style>