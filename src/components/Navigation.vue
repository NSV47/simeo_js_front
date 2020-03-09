<template>
  <v-card height="400" width="256" class="">
    <v-navigation-drawer permanent>
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="title">Application</v-list-item-title>
          <v-list-item-subtitle>subtext</v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list dense nav>
        <v-list-item
          v-for="item in items"
          :key="item.title"
          @click="$router.push(item.path)"
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </v-card>
</template>

<script>
export default {
  name: "Navigation",
  data() {
    return {
      items: [
        { title: "Карта", icon: "mdi-view-dashboard", path: "/" },
        { title: "О проекте", icon: "mdi-image", path: "/about" },
      ],
      right: null
    };
  }
};
</script>