<script setup></script>

<template>
  <v-card
    id="quantities"
    elevation="23"
    class="mt-5 mb-5"
    color="transparent"
    style="margin: auto"
    width="100%"
    height="840px"
  >
    <v-card
      width="80%"
      color="#CDF7CD"
      rounded
      elevation="20"
      style="margin: 30px auto"
    >
      <v-icon class="icon" style="right: 480px; top: 15px"
        >mdi-code-json</v-icon
      >

      <v-icon
        class="icon"
        style="right: 0; bottom: 15px; transform: rotate(0.23turn)"
        >mdi-keyboard-outline</v-icon
      >

      <v-row>
        <v-col cols="6" class="d-flex justify-center align-center">
          <div>
            <h2 class="ml-10">Quantities</h2>
            <ul>
              <li class="d-flex">
                <v-icon> mdi-alert</v-icon>
                <h2 class="ml-2">Problem-solving</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-pencil-outline</v-icon>
                <h2 class="ml-2">Creative thinking</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-account-voice</v-icon>
                <h2 class="ml-2">Sincerity</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-star-shooting-outline</v-icon>
                <h2 class="ml-2">Motivation</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-lock</v-icon>
                <h2 class="ml-2">Loyalty</h2>
              </li>
            </ul>
          </div>
        </v-col>
        <v-divider
          :thickness="2"
          class="mt-5 border-opacity-100"
          color="#8c705a"
          vertical
        ></v-divider>
        <v-col cols="auto" class="d-flex justify-center align-center">
          <div>
            <h2 class="ml-10">Technologies</h2>
            <ul>
              <li class="d-flex">
                <v-icon> mdi-language-csharp</v-icon>
                <h2 class="ml-2">APS.NET Core</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-language-csharp</v-icon>
                <h2 class="ml-2">WPF</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-vuejs</v-icon>
                <h2 class="ml-2">VueJS</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-language-html5</v-icon>
                <h2 class="ml-2">HTML</h2>
              </li>
              <li class="d-flex">
                <v-icon> mdi-language-css3</v-icon>
                <h2 class="ml-2">CSS</h2>
              </li>
            </ul>
          </div>
        </v-col>
      </v-row>
    </v-card>
    <v-card
      width="80%"
      color="#CDF7CD"
      rounded
      elevation="20"
      style="margin: 30px auto"
    >
      <v-row>
        <v-col cols="4" class="d-flex justify-center align-center">
          <v-card
            elevation="24"
            width="100%"
            class="mx-auto ma-10 ml-5"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://static.vecteezy.com/system/resources/previews/007/559/603/original/kid-happy-learning-codding-in-computer-web-coding-for-kids-illustration-coding-its-fun-can-be-used-for-web-banner-poster-social-media-promotion-etc-vector.jpg"
              cover
            ></v-img>

            <v-card-title> Coding 3000+ hours </v-card-title>
          </v-card>
        </v-col>
        <v-col cols="4" class="d-flex justify-center align-center">
          <v-card
            elevation="24"
            width="100%"
            class="mx-auto ma-10"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7JWN-Fog-VKTa1GXVHn1JLxXLhI9Qm60HYw&s"
              cover
            ></v-img>

            <v-card-title> Teamwork </v-card-title>
          </v-card>
        </v-col>
        <v-col cols="4" class="d-flex justify-center align-center">
          <v-card
            elevation="24"
            width="100%"
            class="mx-auto ma-10 mr-5"
            max-width="344"
          >
            <v-img
              height="200px"
              src="https://media.licdn.com/dms/image/D4D12AQErZ5-RkQLLsQ/article-cover_image-shrink_720_1280/0/1695644888972?e=2147483647&v=beta&t=-nbMTQSgrpqJa3AGo6dYK2sngsKE-tv-9ntioc-Zyc0"
              cover
            ></v-img>

            <v-card-title> Responsibility </v-card-title>
          </v-card>
        </v-col>
      </v-row>
    </v-card>
  </v-card>
</template>

<style scoped>
li {
  margin: 20px;
}
h2 {
  color: #8c705a;
  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}
i {
  font-size: xx-large;
  color: #387838;
}
.icon {
  font-size: 100px;
  transform: rotate(-0.07turn);
  position: absolute;

  color: silver;
  opacity: 0.5;
}
</style>
