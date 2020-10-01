<template>
  <v-app class="app-container">
    <NavBar />

    <v-main>
      <router-view></router-view>
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",

  components: {
    NavBar,
    Footer,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  /**background-color: #111; **/
}
</style>
