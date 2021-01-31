<template>
  <div class="h-full relative">
    <LandingPage />
  </div>
</template>

<script>
import LandingPage from "./components/LandingPage.vue";

export default {
  name: "App",
  components: {
    LandingPage,
  },
};
</script>

<style>
#app,
html,
body {
  height: 100vh;
  width: 100vw;
  margin: 0;
  padding: 0;
}
.w-full {
  width: 100%;
}
.h-full {
  height: 100%;
}
.relative {
  position: relative;
}
.grid {
  display: grid;
}
.text-center {
  text-align: center;
}
.p-2 {
  padding: 0.5rem;
}
</style>
