<template>
  <div class="home">
    <HomeBath />
    <HomeState />
    <HomeBathSetting />
    <HomeCleanSetting />
    <HomeReserveSetting />
    <img class="bathstart" src="../assets/play.png" />
  </div>
</template>

<script>
// @ is an alias to /src
import HomeBath from "@/components/HomeBath.vue";
import HomeState from "@/components/HomeState.vue";
import HomeBathSetting from "../components/HomeBathSetting.vue";
import HomeCleanSetting from "../components/HomeCleanSetting.vue";
import HomeReserveSetting from "@/components/HomeReserveSetting.vue";

export default {
  name: "HomeView",
  components: {
    HomeBath,
    HomeState,
    HomeBathSetting,
    HomeCleanSetting,
    HomeReserveSetting,
  },
  data() {},
};
</script>
<style scoped>
.home {
  background-color: cornflowerblue;
  height: 2000px;
}
.bathstart {
  width: 70px;

  position: fixed;
  bottom: 40px;
  right: 20px;
}
</style>