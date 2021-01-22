<template>
  <div id="app">
    <NavSideBar />
    <Header />
    <Content />
  </div>
</template>

<script>
import NavSideBar from "./components/NavSideBar.vue";
import Header from "./components/header.vue";
import Content from "./components/Content.vue";

export default {
  name: "App",
  components: {
    NavSideBar,
    Header,
    Content,
  },
};
</script>

<style>
#app {
  font-family: GoogleSans-Regular;
  font-size: 13px;
  margin: 0px;
}
</style>
