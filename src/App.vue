<script>
import { def } from "@vue/shared";
import Card from "./components/Card.vue";
import Home from "./components/Home.vue";

export default {
  name: "App",
  components: {
    Card,
    Home
  }
};
</script>

<template>
  <div>
    <Home />
    <Card />
  </div>
</template>
