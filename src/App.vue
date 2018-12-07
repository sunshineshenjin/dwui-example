<template>
  <div id="app"><baseTable :rowData="tableData" :columns="columns" /></div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import BaseTable from "dwui/packages/base-table/base-table";
export default {
  name: "App",
  components: {
    HelloWorld,
    BaseTable
  },
  data() {
    return {
      columns: [
        { title: "ID", key: "id", sortable: true, width: 70 },
        { title: "唯一标识", key: "account" },
        { title: "产品名", key: "productName" },
        { title: "类型", key: "typeName" },
        { title: "平台", key: "platformName" },
        { title: "域名", key: "domain" },
        { title: "补充说明", key: "summary" },
        { title: "创建时间", key: "createTime" },
        { title: "更新时间", key: "updateTime" }
      ],
      tableData: []
    };
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
