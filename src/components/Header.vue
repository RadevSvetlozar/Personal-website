<script setup>
import { reactive, computed, ref } from "vue";

const scrollIndex = ref(1);

const scrollTo = (index) => {
  scrollIndex.value = index;
  window.scrollTo(100, window.innerHeight * index);
};
</script>
<template>
  <div
    style="height: 150px; background-color: #cdf7cd"
    class="d-flex align-center"
  >
    <v-toolbar elevation="24">
      <h1 class="ml-15" innerText="<> </>"></h1>
      <v-spacer></v-spacer>
      <v-btn @click="scrollTo(1)">Education</v-btn>
      <v-btn @click="scrollTo(1)">Projects</v-btn>
      <v-btn @click="scrollTo(1)">Quantities</v-btn>
      <v-btn @click="scrollTo(1)">Certificates</v-btn>
      <v-btn @click="scrollTo(1)">Cources</v-btn>
      <v-btn @click="scrollTo(1)">Github</v-btn>
      <v-spacer></v-spacer>
    </v-toolbar>
  </div>
</template>

<style scoped></style>
