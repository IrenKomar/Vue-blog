<template>
  <div id="app">
    <MainPage>
    </MainPage>
  </div>
</template>

<script>
import MainPage from "./components/MainPage.vue";
import { store } from "./common/store.js";

store.getMainPageData();
export default {
  name: "app",
  components: {
    MainPage
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
