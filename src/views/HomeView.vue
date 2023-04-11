<template>
  <div class="home">
    <HomeBath />
    <HomeState />
  </div>
</template>

<script>
// @ is an alias to /src

import HomeBath from "@/components/HomeBath.vue";
import HomeState from "@/components/HomeState.vue";

export default {
  name: "HomeView",
  components: {
    HomeBath,
    HomeState,
  },
  data() {
    return {
      value: true,
    };
  },
};
</script>
