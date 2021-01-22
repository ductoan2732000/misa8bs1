<template>
  <div class="nav-side-bar">
    <div class="logo-bar">
      <div class="logo-bar-logo"></div>
      <div class="logo-bar-icon"></div>
    </div>
    <div class="menu-bar" v-for="(item, index) in DataMenu" :key="index">
      <div class="menu-icon" v-bind:style="item.url"></div>
      <div class="menu-text">{{ item.text }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavSideBar",
  data() {
    return {};
  },
  props: {
    DataMenu: {
      type: Array,
    },
  },
};
</script>

<style>
.nav-side-bar {
  position: relative;
  top: 0;
  left: 0;
  width: 220px;
  height: 100vh;
  background-color: #ffffff;
  border-right: 1px solid #bbbbbb;
}
.logo-bar {
  display: flex;
  align-items: center;
  width: 100%;
  height: 60px;
}
.logo-bar-logo {
  width: 30px;
  height: 30px;
  background-image: url("../assets/img/toggle.png");
  background-size: contain;
  background-position: center;
  background-repeat: no-repeat;
  margin-left: 24px;
}
.logo-bar-icon {
  width: 100%;
  height: 30px;
  margin-left: 10px;
  background-image: url("../assets/img/cukcuk-logo.png");
  background-position: 0 center;
  background-repeat: no-repeat;
  background-size: contain;
}
.menu-bar {
  display: flex;
  padding-left: 24px;
  height: 44px;
  cursor: pointer;
  line-height: 44px;
}
.menu-icon {
  width: 20px;
  height: 20px;
  align-self: center;
  margin-right: 10px;
  background-size: contain;
}
</style>
