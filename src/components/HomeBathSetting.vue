<template>
  <div class="box">
    <div class="title">목욕 설정</div>

    <div id="TempSetting">
      <div style="height: 30px">
        <div class="left_box">목욕 온도</div>
        <div class="right_box">40도</div>
      </div>
      <vue-slider v-model="value" />
    </div>

    <div id="LevelSetting">
      <div style="height: 30px">
        <div class="left_box">물 높이</div>
        <div class="right_box">40%</div>
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
  border-radius: 5%;
  background-color: white;
  margin: 3px;
  padding: 8px;
}
.title {
  height: 30px;
  font-size: 20px;
  font-weight: bold;
}

.left_box {
  float: left;
}
.right_box {
  float: right;
}

#TempSetting {
  margin: 15px;
}

#LevelSetting {
  margin: 15px;
}
</style>