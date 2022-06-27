<template>
  <nav class="mb-14">
    <router-link to="/">Home</router-link> |
    <router-link to="/portfolio">Portfolio</router-link>
  </nav>
  <router-view />
  <Footer />
</template>

<script lang="ts">
import Footer from "@/components/Footer.vue";
import { Options, Vue } from "vue-class-component";

@Options({
  components: {
    Footer,
  },
})
export default class App extends Vue {}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
