<template>
  <v-app>
    <div>
      <layout></layout>
    </div>
  </v-app>
</template>

<script>
// import Map from "./views/Map";
// import About from "./views/About";
import Layout from '@/views/Layout.vue'
export default {
  name: "App",
  components: {
    // Map,
    // About
    Layout
  },
  
  data: () => ({})
};
</script>
