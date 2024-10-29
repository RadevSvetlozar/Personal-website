<script setup>
import {computed} from 'vue'
import { useDisplay } from "vuetify";
const display = useDisplay();
console.log(display.lgAndUp)

const lgAndUp = computed(() => {
  return display.lgAndUp
})

const image = computed(() => {
  return new URL(
          `../assets/profile.jpg`,
          import.meta.url
        ).href;
})
</script>

<template>
  <v-card
    id="main"
    elevation="10"
    rounded="14"
    height="70vh"
    max-height="700px"
    class="mt-3 mb-3 main"
  
  >
  
    <div class="d-none d-md-flex">
      <v-card  class="trapezoid1 d-flex">
        <div class="name" style="top: 150px; right: 30%">
          <h3>Hello, I am</h3>
          <h1>Svetlozar Radev</h1>
          <h3>Full-Stack Developer</h3>
        </div>

        <v-img
          class="image"
           style="top: 150px; right: 3%"
             :src="image"
        >
        </v-img>
      </v-card>

      <v-card color="#F2E3D8" class="trapezoid2"
        ><div class="slogan">
          <h4>Work hard,</h4>
          <h4>Play hard</h4>
        </div>
      </v-card>
    </div>
    <div class="d-sm-flex d-md-none">
      <v-card
      
        width="100%"
        height="400px"
        class="mobile d-flex justify-center align-center"
      >
        <v-row class="ma-10">
          <v-col cols="12"
            ><h3 class="font-style">Hello, I am</h3>
            <h1 class="font-style">Svetlozar Radev</h1>
            <h3 class="font-style">Full-Stack Developer</h3></v-col
          >
          <v-col cols="12">
            <v-avatar size="80%">
              <v-img
                width="100px"
              :src="image"
              >
              </v-img>
            </v-avatar>
          </v-col>
        </v-row>
      </v-card>
    </div>
    <v-icon class="icon" style="left: 480px; top: 15px; font-size: 100px"
      >mdi-monitor-dashboard</v-icon
    >
    <v-icon
      class="icon"
      style="
        font-size: 200px;
        right: 300px;
        bottom: 15px;
        transform: rotate(0.05turn);
      "
      >mdi-card-account-details-outline</v-icon
    >
  </v-card>
</template>

<style scoped>
.main{
  background: rgb(207,241,181);
background: linear-gradient(90deg, rgba(207,241,181,1) 0%, rgba(173,206,132,1) 46%, rgba(207,241,181,1) 95%);
}
.mobile{
  background: rgb(222,226,252);
background: radial-gradient(circle, rgba(222,226,252,1) 0%, rgba(88,91,136,0.5550814075630253) 98%);
}
.font-style {
  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}
.name {
  position: absolute;

  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}
.slogan {
  position: inherit;
  left: 100px;
  top: 125px;
  font-family: "Pacifico", cursive;
  font-weight: 400;
  font-style: normal;
  font-size: large;
}
.icon {
  transform: rotate(-0.05turn);
  position: absolute;

  color: silver;
  opacity: 0.5;
}

.trapezoid1 {
  background: rgb(222,226,252);
  background: radial-gradient(circle, rgba(222,226,252,1) 0%, rgba(88,91,136,0.5550814075630253) 98%);
  height: 500px;
  width: 100%;
  position: absolute;
  z-index: 2;
  clip-path: polygon(51% 0, 100% 0%, 100% 100%, 23% 100%);
}

.image {
  position: absolute;
  top: 30%;
  right: 50px;
  width: 200px;
  height: 200px;
  clip-path: polygon(
    50% 0%,
    80% 10%,
    100% 35%,
    100% 70%,
    80% 90%,
    50% 100%,
    20% 90%,
    0% 70%,
    0% 35%,
    20% 10%
  );
}
.image1 {
  margin: 0 auto;
  width: 100px;
  height: 100px;
}

.trapezoid2 {
  background: rgb(222,226,252);
background: radial-gradient(circle, rgba(222,226,252,1) 0%, rgba(88,91,136,0.5550814075630253) 98%);
  height: 500px;
  position: absolute;
  z-index: 2;
  width: 100%;
  clip-path: polygon(10% 18%, 10% 78%, 30% 17%);
}
</style>
