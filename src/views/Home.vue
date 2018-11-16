<template>
  <div class="home">
    <div id="btn" @click='jump_about' v-if="logo==false">
      登录
      <!-- <router-link to="/about"></router-link> -->
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "home",
  components: {},
  data() {
    return {
      logo: false
    };
  },
  methods: {
    jump_about() {
      this.logo = true;
      // 字符串
      this.$router.push("/about");

      // 对象
      // this.$router.push({ path: '/home/first' })

      // 命名的路由
      // this.$router.push({ name: 'home', params: { userId: wise }})
    }
  }
};
</script>
<style lang="less">
#btn {
  width: 300px;
  height: 30px;
  background: aquamarine;
  margin: 0 auto;
  line-height: 30px;
  font-size: 18px;
  color: #fff;
  font-weight: bold;
  text-align: center;
  a {
    width: 100%;
    height: 100%;
    display: inline-block;
    line-height: 30px;
    font-size: 18px;
    color: #fff;
    font-weight: bold;
  }
}
</style>
