<template>
  <div class="h-full w-full relative">
    <div id="map" style="height: 100%; width: 100%; inset: 0px;"></div>
  </div>
</template>

<script>
let mapboxgl = require("mapbox-gl/dist/mapbox-gl.js");
mapboxgl.accessToken =
  "pk.eyJ1IjoibWFya29kdXJhc2lub3ZpYyIsImEiOiJja2tsZWRsMTYyZnkzMnVtbmNydTByd2hjIn0.Z3iU9zKwh5dt6_0pAmc73Q";

export default {
  name: "Map",
  mounted() {
    let map = new mapboxgl.Map({
      container: "map",
      style: "mapbox://styles/mapbox/streets-v11",
      center: [-0.1278, 51.5074],
      zoom: 8,
    });
    // console.log(map);

    new mapboxgl.Marker().setLngLat([-74.5, 40]).addTo(map);
  },
};
</script>

<style scoped></style>
