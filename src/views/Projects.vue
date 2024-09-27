<script setup>
import barber from "../assets/barber.png"; // => or relative path
import shopping from "../assets/shopping-list-app.png"; // => or relative path
const getImage = (link) => {
  return new URL(link, import.meta.url).href;
};
</script>

<template>
  <v-card
    id="projects"
    elevation="15"
    rounded="14"
    height="auto"
    max-height="700px"
    class="main mt-3 mb-3"
  >
    <v-icon
      class="icon"
      style="left: 40%; bottom: 40%; transform: rotate(0.05turn)"
      >mdi-folder-file-outline</v-icon
    >
    <v-row class="d-flex justify-center">
      <v-col cols="auto"> <h1 class="pt-5">Projects</h1></v-col>
    </v-row>

    <v-row class="d-flex justify-center align-center">
      <v-col cols="5">
        <v-card
          elevation="24"
          color="#F2E3D8"
          class="ma-10 d-flex align-center"
          height="250px"
        >
          <div>
            <v-card-title>
              <h3>Домашен майстор /Homemaker/</h3>
            </v-card-title>
            <v-card-subtite class="pa-2"
              >The platform helps everyone find their home handyman by type of
              activity and location</v-card-subtite
            >
          </div>
        </v-card>
      </v-col>
      <v-divider
        :thickness="2"
        class="mt-5 border-opacity-100"
        color="#8c705a"
        vertical
      ></v-divider>
      <v-col cols="5">
        <v-card elevation="24" class="ma-10" height="auto">
          <v-img
            cover
            src="https://bootstrapmade.com/content/templatefiles/Impact/Impact-bootstrap-website-template-md.webp"
          />
        </v-card>
      </v-col>
    </v-row>
    <v-row class="mt-10 d-flex justify-center align-center">
      <v-col cols="5">
        <v-card elevation="24" class="ma-10" height="auto">
          <v-img cover :src="barber" />
        </v-card>
      </v-col>
      <v-divider
        :thickness="2"
        class="mt-5 border-opacity-100"
        color="#8c705a"
        vertical
      ></v-divider>

      <v-col cols="5">
        <v-card
          elevation="24"
          color="#F2E3D8"
          class="ma-10 d-flex align-center"
          height="250px"
        >
          <div>
            <v-card-title>
              <h3>Miro Boev - BarberShop</h3>
            </v-card-title>
            <v-card-subtite class="pa-2"
              >Barbershop website with booking</v-card-subtite
            >
          </div>
        </v-card>
      </v-col>
    </v-row>
    <v-row class="mt-10 d-flex justify-center align-center">
      <v-col cols="5">
        <v-card
          elevation="24"
          color="#F2E3D8"
          class="ma-10 d-flex align-center"
          height="250px"
        >
          <div>
            <v-card-title>
              <h3>Shopping list app</h3>
            </v-card-title>
            <v-card-subtite class="pa-2"
              >Progressive web app in which a person can add to a list the
              products needed for purchase</v-card-subtite
            >
          </div>
        </v-card>
      </v-col>
      <v-divider
        :thickness="2"
        class="mt-5 border-opacity-100"
        color="#8c705a"
        vertical
      ></v-divider>
      <v-col cols="5">
        <v-card elevation="24" class="ma-10" height="auto">
          <v-img cover :src="shopping" />
        </v-card>
      </v-col>
    </v-row>
  </v-card>
</template>

<style scoped>
h1,
h3 {
  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}

.icon {
  font-size: 400px;
  transform: rotate(-0.01turn);
  position: absolute;

  color: silver;
  opacity: 0.6;
}
</style>
