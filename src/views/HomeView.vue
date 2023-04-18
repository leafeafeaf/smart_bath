<template>
  <div class="home">
    <HomeBath />
    <HomeState />
    <HomeBathSetting />
    <HomeCleanSetting />
    <HomeReserveSetting />
    <Footer />
    <img class="bathstart" src="../assets/play.png" v-on:click="bStart" />
  </div>
</template>

<script>
// @ is an alias to /src
import HomeBath from "@/components/HomeBath.vue";
import HomeState from "@/components/HomeState.vue";
import HomeBathSetting from "../components/HomeBathSetting.vue";
import HomeCleanSetting from "../components/HomeCleanSetting.vue";
import HomeReserveSetting from "@/components/HomeReserveSetting.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "HomeView",
  components: {
    HomeBath,
    HomeState,
    HomeBathSetting,
    HomeCleanSetting,
    HomeReserveSetting,
    Footer,
  },
  data() {},
  methods: {
    //목욕 시작 명령
    bStart: function () {
      console.log("Click mbath");
    },
  },
};
</script>
<style scoped>
.home {
  background-color: cornflowerblue;
  height: 2000px;
}
.bathstart {
  width: 50px;
  position: fixed;
  bottom: 80px;
  right: 20px;
  z-index: 1;
}
</style>