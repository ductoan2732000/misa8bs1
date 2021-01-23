<template>
  <div id="app">
    <NavSideBar v-bind:DataMenu="DataMenu"></NavSideBar>
    <div class="side-right">
      <Header />
      <Content />
    </div>
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
          url: "../assets/icon/icons8-sort-24.png",

          text: "Tổng quan",
        },
        {
          url: "background-image: url('../assets/icon/icons8-sort-24.png');",
          text: "Báo cáo",
        },
        {
          url: "background-image: url('../assets/icon/icons8-sort-24.png');",
          text: "Mua hàng",
        },
        {
          url: "background-image: url('../assets/icon/icons8-sort-24.png');",
          text: "Danh mục khách hàng",
        },
        {
          url: "background-image: url('../assets/icon/icons8-sort-24.png');",
          text: "Danh mục khách hàng",
        },
        {
          url: "background-image: url('../assets/icon/icons8-sort-24.png');",
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
