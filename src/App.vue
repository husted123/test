<template>
  <Navbar />
  <router-view />
  <Footer />
</template>
<script>
import Navbar from "../src/components/Navbar";
import Footer from "../src/components/Footer";

export default {
  components: {
    Navbar,
    Footer
  },
  methods: {}
};
</script>
<style lang="scss">
#app {
  font-family: Arial, sans-serif, Avenir, Helvetica;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #212121;
}
body {
  margin: 0;
}
.home {
  margin-top: 80px;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.wedio-logo {
  max-width: 800px;
  max-height: 400px;
}
h1 {
  margin-top: 100px;
}
</style>
