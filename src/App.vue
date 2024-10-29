<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Main from "./views/Main.vue";
import Education from "./views/Education.vue";
import Quantities from "./views/Quantities.vue";
import Projects from "./views/Projects.vue";
import Certificates from "./views/Certificates.vue";
</script>

<template>
  <v-app>
    <div class="main1">
      <Header></Header>
      <Main></Main>
      <Education></Education>
      <Quantities></Quantities> 
      <Certificates></Certificates> 
       <!-- <Projects></Projects> -->
      <Footer></Footer>
    </div>
  </v-app>
</template>

<style>
html {
  scroll-behavior: smooth;
}
.main1 {
  max-width: 1200px;
  margin: 0 auto;
  background-color: #ededed;
}
</style>
