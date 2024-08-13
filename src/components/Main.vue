<script setup></script>

<template>
  <v-card height="600px" class="main mt-3 mb-3" color="#CDF7CD">
    <v-card color="#F2E3D8" class="trapezoid1 d-flex">
      <h3>Hello, I am</h3>
      <h2>Svetlozar Radev</h2>
      <h4>Full-Stack Developer</h4>
      <v-img
        class="image"
        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR8HrGomjMzPa4p16svxviHG6hpdrrJ8YyYjw&s"
      >
      </v-img>
    </v-card>
    <v-card color="#F2E3D8" class="trapezoid2"> 2</v-card>
  </v-card>
</template>

<style scoped>
.main {
  position: relative;
}
.trapezoid1 {
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
.trapezoid1 h3 {
  position: absolute;
  top: 150px;
  right: 410px;
}
.trapezoid1 h2 {
  position: absolute;
  top: 190px;
  right: 410px;
}
.trapezoid1 h4 {
  position: absolute;
  top: 250px;
  right: 410px;
}
.trapezoid2 {
  height: 500px;
  position: absolute;
  z-index: 2;
  width: 100%;
  clip-path: polygon(10% 18%, 10% 78%, 30% 17%);
}
</style>
