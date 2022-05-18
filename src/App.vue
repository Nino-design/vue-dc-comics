<template>
  <div id="app">
    <!--HEADER-->
    <AppHeader />
    <main>
      <h1>Content goes here</h1>
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

export default {
  name: "App",
  components: {
    AppHeader,
    AppMainLinks,
    AppTopFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
