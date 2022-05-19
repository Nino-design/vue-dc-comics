<template>
  <div id="app">
    <!--HEADER-->
    <AppHeader />
    <main>
      <AppJumbo />
      <AppComicsList/>
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
import AppComicsList from "./components/AppComicsList.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppJumbo,
    AppMainLinks,
    AppTopFooter,
    AppBottomFooter,
    AppComicsList,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
