<template>
  <div id="app">
    <HeaderPage></HeaderPage>
    <router-view />
    <FooterPage></FooterPage>
  </div>
</template>

<style>
body {
  margin: 0;
  padding: 0;
  font-family: "Muli", sans-serif;
}
</style>

<script>
import HeaderPage from "./components/HeaderPage";
import FooterPage from "./components/FooterPage";

export default {
  components: {
    HeaderPage,
    FooterPage
  }
};
</script>
