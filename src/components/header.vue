<template>
  <div class="header"></div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {};
  },
};
</script>

<style>
.header {
  position: absolute;
  top: 0;
  right: 0;
  display: flex;
  align-items: center;
  width: calc(100% - 221px);
  height: 60px;
  border-bottom: 1px solid #bbbbbb;
}
</style>
