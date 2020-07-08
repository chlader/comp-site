<template>
  <v-app>
    <div class="nav">
      <router-link style="margin-left: 40px; color: black;" to="/">R^2 Tech</router-link>
      <div class="links">
        <router-link to="/about">About</router-link>
        <router-link to="/project">Projects</router-link>
        <router-link to="/contact">Contact Us</router-link>
      </div>
    </div>
    <router-view />
    <Footer></Footer>
  </v-app>
</template>

<script>
import Footer from "./views/Footer";

export default {
  name: "App",
  components: {
    Footer
  }
};
</script>

<style>
.nav {
  height: 40px;
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
}

a {
  margin: 0 20px;
  text-decoration: none;
}
</style>
