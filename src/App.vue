<template>
  <navbar></navbar>
  <h1>Welcome to Carshowroom</h1>
  <div class="container">
    <gallerycard></gallerycard>
  </div>
  <layoutfooter></layoutfooter>
</template>

<script>
import navbar from "./components/layout/Navbar.vue";
import layoutfooter from "./components/layout/Footer.vue";
import gallerycard from "./components/GalleryCard";

export default {
  name: "App",
  components: {
    navbar,
    layoutfooter,
    gallerycard,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
