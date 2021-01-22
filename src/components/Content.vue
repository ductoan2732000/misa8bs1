<template>
  <div class="content">
    <div class="header-content">
      <div class="title-header">Danh sachs khách hàng</div>
      <div class="add-header">
        <button class="btn-add">
          <div class="btn-add-icon"></div>
          <div class="btn-add-text">Thêm khách hàng</div>
        </button>
      </div>
    </div>
    <div class="filter-content">
      <div class="filter-left">
        <input
          type="text"
          class="icon-search input-search"
          placeholder="Tìm kiếm theo Mã, Tên Khác"
        />
      </div>
      <div class="filtet-right">
        <button class="btn-fresh"></button>
      </div>
    </div>
    <div class="data-content"></div>
    <div class="pagging-bar">
      <div class="pagging-info"></div>
      <div class="pagging-option"></div>
      <div class="pagging-recode"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Conent",
  data() {
    return {};
  },
};
</script>

<style>
.content {
  position: absolute;
  top: 61px;
  right: 0px;
  width: calc(100% - 253px);
  height: auto;
  background-color: #ffffff;
  padding: 16px;
}
.header-content {
  padding: 8px 0 16px 0;
  display: flex;
  align-items: center;
}
.filter-content {
  width: 100%;
  display: flex;
  align-items: center;
  height: 40px;
}
.data-content {
  height: calc(100vh - 246px);
}
.title-header {
  font-size: 20px;
  font-weight: bold;
}
.add-header {
  position: absolute;
  right: 16px;
}
.btn-add {
  display: flex;
  align-items: center;
  background-color: #019160;
  border-radius: 4px;
  height: 40px;
  font-size: 13px;
  color: #ffffff;
  font-family: GoogleSans-Regular;
  padding-left: 16px;
  padding-right: 16px;
  outline: none;
  border: none;
  cursor: pointer;
  min-width: 100px;
  justify-content: center;
}
.btn-add-icon {
  background-position: center;
  width: 16px;
  height: 16px;
  background-image: url("../assets/icon/add.png");
}
.btn-add-text {
  margin-left: 8px;
}
.input-search {
  width: 200px;
  height: 40px;
  box-sizing: border-box;
  padding-left: 40px;
  padding-right: 16px;
  outline: none;
  border-radius: 4px;
  border: 1px solid #bbbbbb;
}
.input-search::placeholder {
  font-size: 11px;
  color: #bbbbbb;
}
.input-search:focus {
  border: 1px solid #01b075;
}
.icon-search {
  background-image: url("../assets/icon/search.png");
  background-repeat: no-repeat;
  background-position: 16px center;
  background-size: 16px;
}
.filter-left {
  width: 200px;
  height: 40px;
}
.filtet-right {
  position: absolute;
  right: 16px;
}
.btn-fresh {
  background-image: url("../assets/icon/refresh.png");
  background-repeat: no-repeat;
  width: 40px;
  height: 40px;
  background-position: center;
  border: 1px solid #bbbbbb;
  outline: none;
  border-radius: 4px;
  cursor: pointer;
}
.btn-fresh:hover {
  background-color: #bbbbbb;
}
</style>
