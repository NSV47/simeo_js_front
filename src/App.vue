<template>
  <div>
    <h1>Мое приложение</h1>
    <nav>
      <ul>
        <li>
          <router-link to="/">Карта</router-link>
        </li>
        <li>
          <router-link to="/about">О проекте</router-link>
        </li>
      </ul>
    </nav>
    <!-- <Map v-if="page === 'Map'"></Map>
    <About v-if="page === 'About'"></About> -->
    <router-view></router-view>
  </div>
  
</template>

<script>
// import Map from "./views/Map";
// import About from "./views/About";

export default {
  name: "App",
  components: {
    // Map,
    // About
  },

  data: () => ({
    page: "About"
  })
};
</script>
