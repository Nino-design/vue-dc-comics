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
    </footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainLinks from "./components/AppMainLinks.vue";
import AppTopFooter from "./components/AppTopFooter.vue";
import AppJumbo from "./components/AppJumbo.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMainLinks,
    AppTopFooter,
    AppJumbo,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
