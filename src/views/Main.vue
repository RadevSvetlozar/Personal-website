<script setup></script>

<template>
  <v-card
    id="main"
    elevation="10"
    rounded="14"
    height="70vh"
    class="main mt-3 mb-3"
    color="#CDF7CD"
  >
    <v-card color="#F2E3D8" class="trapezoid1 d-flex">
      <div class="name">
        <h3>Hello, I am</h3>
        <h1>Svetlozar Radev</h1>
        <h3>Full-Stack Developer</h3>
      </div>

      <v-img
        class="image"
        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR8HrGomjMzPa4p16svxviHG6hpdrrJ8YyYjw&s"
      >
      </v-img>
    </v-card>

    <v-card color="#F2E3D8" class="trapezoid2"
      ><div class="slogan">
        <h3>Work hard,</h3>
        <h3>Play hard</h3>
      </div>
    </v-card>

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
.name {
  position: absolute;
  top: 150px;
  right: 410px;

  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}
.slogan {
  position: inherit;
  left: 130px;
  top: 125px;
  font-family: "Pacifico", cursive;
  font-weight: 400;
  font-style: normal;
  font-size: x-large;
}
.icon {
  transform: rotate(-0.05turn);
  position: absolute;

  color: silver;
  opacity: 0.5;
}
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

.trapezoid2 {
  height: 500px;
  position: absolute;
  z-index: 2;
  width: 100%;
  clip-path: polygon(10% 18%, 10% 78%, 30% 17%);
}
</style>
