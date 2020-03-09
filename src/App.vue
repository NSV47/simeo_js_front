<template>
  <v-app>
    <div>
      <Layout></Layout>
    </div>
  </v-app>
</template>

<script>
// import Map from "./views/Map";
// import About from "./views/About";
import Layout from '@/views/Layout'
export default {
  name: "App",
  components: {
    // Map,
    // About
    Layout
  },

  data: () => ({
    page: "About"
  })
};
</script>
