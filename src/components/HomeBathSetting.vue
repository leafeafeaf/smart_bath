<template>
  <div class="box">
    <div class="title">목욕 설정</div>
    <div id="TempSetting">
      <div>
        <p>목욕 온도</p>
        <p>40도</p>
      </div>
      <vue-slider v-model="value" />
    </div>
    <div id="LevelSetting">
      <div>
        <p>물 높이</p>
        <p>40%</p>
      </div>
      <vue-slider v-model="value" />
    </div>
  </div>
</template>
<script>
import VueSlider from "vue-slider-component";
import "vue-slider-component/theme/default.css";

export default {
  components: {
    VueSlider,
  },
};
</script>
<style scoped>
.box {
  border-radius: 10%;
  background-color: crimson;
}
</style>