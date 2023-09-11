<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";
import AppCard from "./components/AppCard.vue";


export default {
  components: { AppHeader, AppMain, AppFooter, AppCard},
};
</script>

<template>
  <AppHeader />
  <AppCard />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
