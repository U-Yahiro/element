<template>
  <el-menu
    default-active="1"
    class="el-menu-vertical-demo"
    @open="handleOpen"
    @close="handleClose"
    background-color="rgba(15, 39, 62, 1);"
    text-color="#fff"
    active-text-color="#ffd04b"
    :collapse="isCollapse" >
    <el-submenu index="1">
      <template slot="title">
        <i class="el-icon-location"></i>
        <span slot="title">Navigator One</span>
      </template>
      <el-menu-item-group>
        <span slot="title">Group One</span>
        <el-menu-item index="1-1">item one</el-menu-item>
        <el-menu-item index="1-2">item two</el-menu-item>
      </el-menu-item-group>
      <el-menu-item-group title="Group Two">
        <el-menu-item index="1-3">item three</el-menu-item>
      </el-menu-item-group>
      <el-submenu index="1-4">
        <span slot="title">item four</span>
        <el-menu-item index="1-4-1">item one</el-menu-item>
      </el-submenu>
    </el-submenu>
    <el-menu-item index="2">
      <i class="el-icon-menu"></i>
      <span slot="title">Navigator Two</span>
    </el-menu-item>
    <el-menu-item index="4">
      <i class="el-icon-setting"></i>
      <span slot="title">Navigator Four</span>
    </el-menu-item>
    <el-menu-item index="4">
      <i class="el-icon-setting"></i>
      <span slot="title">Navigator Four</span>
    </el-menu-item>
    <el-menu-item index="4">
      <i class="el-icon-setting"></i>
      <span slot="title">Navigator Four</span>
    </el-menu-item>
    <el-menu-item index="4">
      <i class="el-icon-setting"></i>
      <span slot="title">Navigator Four</span>
    </el-menu-item>
    <p class="spacer">
      <i class="el-icon-s-unfold"></i>
    <el-button
      type="primary"
      plain
      @click="isCollapse = !isCollapse"
    ></el-button>
    </p>
  </el-menu>
</template>

<style>
.el-menu-vertical-demo:not(.el-menu--collapse) {
  width: 200px;
  min-height: 400px;
}
</style>

<script>
export default {
  data() {
    return {
      isCollapse: true,
    };
  },
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>

<style scoped>
.spacer {
  position: absolute;
  margin-top: 250px;
  padding-left: 10px;
}

.el-menu {
    border-right: solid 1px #e6e6e6;
    list-style: none;
    position: relative;
    margin: 0;
    padding-left: 0;
    background-color:rgba(15, 39, 62, 1);
}
</style>
