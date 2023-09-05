<script>
import { def } from "@vue/shared";
import Home from "./components/Home.vue";
import Card from "./components/Card.vue";

export default {
  name: "App",
  components: {
    Home,
    Card
  },
  data() {
    return {
      showHome: true
    };
  }
};
</script>

<template>
  <div>
    <Home v-if="showHome" />
    <Card v-else />
  </div>
</template>
