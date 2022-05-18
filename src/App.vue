<template>
  <div id="app">
    <!--HEADER-->
    <AppHeader />
    <main>
      <AppJumbo />
    </main>
    <AppMainLinks />
    <footer>
      <AppTopFooter />
      <AppBottomFooter/>
    </footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbo from "./components/AppJumbo.vue";
import AppMainLinks from "./components/AppMainLinks.vue";
import AppTopFooter from "./components/AppTopFooter.vue";
import AppBottomFooter from "./components/AppBottomFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppJumbo,
    AppMainLinks,
    AppTopFooter,
    AppBottomFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
