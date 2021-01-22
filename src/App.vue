<template>
  <div id="app">
    <NavSideBar v-bind:DataMenu="DataMenu"></NavSideBar>
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
  data() {
    return {
      DataMenu: [
        {
          url:
            "background-image: url('./assets/icon/icons8-alert-50 (1).png');",
          text: "Tổng quan",
        },
        {
          url: "url('../assets/icon/search.png')",
          text: "Báo cáo",
        },
        {
          url: "url('../assets/icon/search.png')",
          text: "Mua hàng",
        },
        {
          url: "url('../assets/icon/search.png')",
          text: "Danh mục khách hàng",
        },
        {
          url: "url('../assets/icon/search.png')",
          text: "Danh mục khách hàng",
        },
        {
          url: "url('../assets/icon/search.png')",
          text: "Thiết lập hệ thống",
        },
      ],
    };
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
