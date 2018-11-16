<template>
  <div id="app">
    <router-view/>
  </div>
</template>
<script>
export default {
  name: "app",
  components: {},
  data() {
    return {
      logo: true
    };
  }
};
</script>
<style lang="less">
@import url(css/style.css);
@import url(css/reset.css);
@import url(css/common.css);
@import url(css/theme-custom.css);
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  background: #fff;
  position: relative;
}
</style>
