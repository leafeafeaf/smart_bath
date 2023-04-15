<template>
  <div class="box">
    <div class="title">
      <div class="left_box">청소 설정</div>
      <Toggle v-model="value" class="right_box" />
    </div>
    <div>
      <scroll-picker :options="options" v-model="selections" />
    </div>
  </div>
</template>
<script>
import "@vueform/toggle/themes/default.css";
import { defineComponent, reactive, toRefs } from "vue";

const scrollpickerOptions = [
  [
    {
      label: "5",
      value: 5,
    },
    {
      label: "10",
      value: 10,
    },
    {
      label: "15",
      value: 15,
    },
    {
      label: "20",
      value: 20,
    },
    {
      label: "25",
      value: 25,
    },
    {
      label: "30",
      value: 30,
    },
    {
      label: "35",
      value: 35,
    },
    {
      label: "40",
      value: 40,
    },
    {
      label: "45",
      value: 45,
    },
    {
      label: "50",
      value: 50,
    },
    {
      label: "55",
      value: 55,
    },
    {
      label: "60",
      value: 60,
    },
  ],
];

export default defineComponent({
  setup() {
    const state = reactive({
      options: scrollpickerOptions,
      selections: [30],
      value: true,
    });
    return {
      ...toRefs(state),
    };
  },
});
</script>
<style scoped>
.box {
  border-radius: 10%;
  background-color: crimson;
}
.title {
  height: 30px;
}
.left_box {
  float: left;
}
.right_box {
  float: right;
}
</style>