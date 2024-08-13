<script setup>
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Education from "./components/Education.vue";
import Quantities from "./components/Quantities.vue";
import Projects from "./components/Projects.vue";
</script>

<template>
  <div class="main">
    <Header></Header>
    <Main></Main>
    <Education></Education>
    <Quantities></Quantities>
    <Projects></Projects>
  </div>
</template>

<style scoped>
.main {
  max-width: 1200px;
  margin: 0 auto;
  background-color: #ededed;
}
</style>
