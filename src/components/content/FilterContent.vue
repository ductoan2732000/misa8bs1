<template>
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
</template>

<script>
export default {
  name: "FilterContent",
};
</script>

<style>
.filter-content {
  width: 100%;
  display: flex;
  align-items: center;
  height: 40px;
}
.filter-left {
  width: 200px;
  height: 40px;
}
.filtet-right {
  position: absolute;
  right: 16px;
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
  background-image: url("../../assets/icon/search.png");
  background-repeat: no-repeat;
  background-position: 16px center;
  background-size: 16px;
}
.btn-fresh {
  background-image: url("../../assets/icon/refresh.png");
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