<script setup>
import { watch, reactive, computed, ref, onMounted, onUnmounted } from "vue";

const scrollIndex = ref(0);

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
    <v-row class="d-flex justify-center">
      <v-col class="d-flex-column align-start" cols="5"
        ><h2>Powered by Svetlozar Radev</h2>
        <h4>Full-Stack developer</h4>
        <h4>© 2024 All rights reserved.</h4>
      </v-col>
      <v-divider vertical></v-divider>
      <v-col class="d-flex align-end" cols="5"
        ><h2>Love your job, learn more skills</h2></v-col
      >
    </v-row>
  </div>
</template>

<style scoped>
h2, h4 {
  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}
</style>
