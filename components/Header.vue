<template>
<el-menu
  :default-active="activeIndex2"
  class="el-menu-demo"
  mode="horizontal"
  @select="handleSelect"
  background-color="rgba(15, 39, 62, 1);"
  text-color="#fff"
  active-text-color="#ffd04b">
  <el-menu-item index="1"></el-menu-item>
  <!-- <el-menu-item index="3" disabled></el-menu-item> -->
  <!-- <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">Orders</a></el-menu-item> -->
</el-menu>

</template>

<script>
  export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped>
header.el-header {
    padding-left: 0px;
    padding-right: 0px;
    box-sizing: border-box;
    flex-shrink: 0;
}

menu {
    height: 60px;
    padding-left: 0px;
    padding-right: 0px;
    position: fixed;
}

el-menu {
    position: fixed;
}
</style>