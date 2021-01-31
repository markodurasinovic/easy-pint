<template>
  <div
    class="h-full grid relative"
    style="grid-template-rows: max-content auto;"
  >
    <Header />
    <Map />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Map from "@/components/Map.vue";

export default {
  name: "LandingPage",
  components: {
    Header,
    Map,
  },
};
</script>

<style lang="scss" scoped></style>
