<script setup></script>

<template>
  <v-card
    id="main"
    elevation="10"
    rounded="14"
    height="70vh"
    max-height="700px"
    class="mt-3 mb-3"
    color="#CDF7CD"
  >
    <div class="d-none d-sm-flex">
      <v-card color="#F2E3D8" class="trapezoid1 d-flex">
        <div class="name" style="top: 150px; right: 30%">
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
    </div>

    <v-card
      color="#F2E3D8"
      width="100%"
      height="400px"
      class="d-flex justify-center align-center"
    >
      <v-card>
        <h3>Hello, I am</h3>
        <h1>Svetlozar Radev</h1>
        <h3>Full-Stack Developer</h3>

        <v-img
          width="100px"
          src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR8HrGomjMzPa4p16svxviHG6hpdrrJ8YyYjw&s"
        >
        </v-img>
      </v-card>
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
  height: 500px;
  position: absolute;
  z-index: 2;
  width: 100%;
  clip-path: polygon(10% 18%, 10% 78%, 30% 17%);
}
</style>
