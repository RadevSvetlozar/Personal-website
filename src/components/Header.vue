<script setup>
import { watch, reactive, computed, ref, onMounted, onUnmounted } from "vue";
import { useGoTo } from "vuetify";
const scrollIndex = ref(0);

const scrollTo = (index) => {
  scrollIndex.value = index;
  window.scrollTo(100, window.innerHeight * index);
};

const goTo = useGoTo();

const options = computed(() => {
  return {
    container: "#goto-container-example",
    duration: 300,
    easing: "easeInOutCubic",
    offset: 0,
  };
});
</script>
<template>
  <div
    id="header"
    style="height: 150px; background-color: #cdf7cd"
    class="d-flex align-center"
  >
    <v-toolbar elevation="24">
      <h1 class="ml-15" innerText="<> </>"></h1>
      <v-spacer></v-spacer>
      <v-btn @click="goTo('#education', options)"><h2>Education</h2></v-btn>
      <v-btn @click="goTo('#quantities', options)"><h2>Quantities</h2> </v-btn>
      <v-btn @click="goTo('#certificates', options)"
        ><h2>Certificates</h2></v-btn
      >
      <v-btn @click="goTo('#projects', options)"><h2>Projects</h2></v-btn>
      <v-btn href="https://github.com/RadevSvetlozar" target="_blank"
        ><h2>Github</h2></v-btn
      >

      <v-spacer></v-spacer>
    </v-toolbar>
    <v-btn
      style="position: fixed; right: 150px; bottom: 30px"
      color="#CDF7CD"
      size="x-large"
      icon="mdi-arrow-up-bold-circle-outline"
      @click="goTo('#header', options)"
    >
    </v-btn>
  </div>
</template>

<style scoped>
h2 {
  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}
</style>
