<template>
<el-container>
  <el-header>
    <Header />
  </el-header>
  <el-container>
       <SideNav />
    <el-main id="main">Main
      <Nuxt />
    </el-main>
  </el-container>
</el-container>
</template>

<script>
import  SideNav from "~/components/SideNav";
import  Header from "~/components/Header";

export default {
  components:{
    SideNav,
    Header
  }
}
</script>
<style>
main {
  transition: margin-left .5s;
  padding: 20px;
}

.el-header {
    padding: 0 0px;
    box-sizing: border-box;
    flex-shrink: 0;
}

.main-layout {
  position: relative;
}

.el-menu-layout {
    position: fixed;
    background: grey !important;
    left: 0;
    margin-top: 60px;
}

.el-header {
    position: fixed;
    background-color: white;
    height: 12%;
    top: 0;
    left: 0;
   right: 0;
}

.main-container {
  margin-top:60px;
  margin-left: 100px;
}

html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
