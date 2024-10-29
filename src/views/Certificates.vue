<script setup>
import { reactive, ref, computed } from "vue";
import { useGoTo } from "vuetify";
const certificates = reactive([
  {
    text: "Programming Basics with C# - October 2019",
    link: "basic.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "C# Fundamentals - January 2020",
    link: "fundamental.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "Databases Basics - MS SQL Server - May 2020",
    link: "database_basic.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "C# Advanced - May 2020",
    link: "advanced.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "Entity Framework Core - June 2020",
    link: "EFjpg.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "C# OOP - June 2020",
    link: "oop.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "C# Web Basics - September 2020",
    link: "web_basics.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "ASP.NET Core - October 2020",
    link: "asp.jpg",
    icon: "mdi-language-csharp",
  },
  {
    text: "JS Advanced - January 2021",
    link: "js_advanved.jpg",
    icon: "mdi-language-csharp",
  },
]);
const cources = reactive([
  {
    text: "WPF Essentials",
    link: "basic.jpg",
    icon: "mdi-language-csharp",
  },
  { text: "VueJS", link: "basic.jpg", icon: "mdi-vuejs" },
  { text: "Angular", link: "basic.jpg", icon: "mdi-angular" },
  { text: "ExpressJS", link: "basic.jpg", icon: "mdi-nodejs" },
  {
    text: "HTML & CSS",
    link: "basic.jpg",
    icon: "mdi-language-html5",
  },
]);
const getImgUrl = (imageNameWithExtension) =>
  new URL(`../assets/${imageNameWithExtension}`, import.meta.url).href;
const selectedCertificateLink = ref(certificates[0].link);
const clickOnItem = (text) => {
  goTo("#imgCont", options);
  for (const certificate of certificates) {
    if (certificate.text !== text) {
      document.getElementById(certificate.text).style.zIndex = "1";
    } else {
      document.getElementById(certificate.text).style.zIndex = "10";
    }
  }
};

const goTo = useGoTo();

const options = computed(() => {
  return {
    container: "#goto-container-example",
    duration: 100,
    easing: "easeInOutCubic",
    offset: 0,
  };
});
</script>
<template>
  <v-card id="certificates" elevation="15" rounded="14" class="main mt-3 mb-3">
    <v-icon
      class="icon"
      style="left: 510px; bottom: 150px; transform: rotate(0.05turn)"
      >mdi-folder-text-outline</v-icon
    >
    <v-row>
      <v-col cols="12" md="6">
        <v-card elevation="24" class="ma-3" rounded>
          <v-list density="compact" color="red">
            <v-list-header><h1 class="ma-2">Certificates</h1></v-list-header>
            <v-list-item
              v-for="(certificate, i) in certificates"
              :key="i"
              :value="certificate.text"
              color="primary"
              class="pa-2"
              @click="clickOnItem(certificate.text)"
            >
              <template v-slot:prepend>
                <v-icon :icon="certificate.icon"></v-icon>
              </template>
              <v-list-item-title v-text="certificate.text"></v-list-item-title>
            </v-list-item>
          </v-list>
        </v-card>
        <v-card elevation="24" class="ma-3" rounded>
          <v-list density="compact">
            <v-list-header><h1 class="ma-2">Cources</h1></v-list-header>
            <v-list-item
              v-for="(course, i) in cources"
              :key="i"
              :value="course.text"
              color="primary"
              class="pa-2"
            >
              <template v-slot:prepend>
                <v-icon :icon="course.icon"></v-icon>
              </template>
              <v-list-item-title v-text="course.text"></v-list-item-title>
            </v-list-item>
          </v-list>
        </v-card>
      </v-col>
      <v-col cols="12" md="6" class="d-flex justify-start align-center">
        <div id="imgCont" class="img-container">
          <v-card
            v-for="(certificate, i) in certificates"
            :key="i"
            elevation="20"
            class="img border"
            :style="{ left: i * 20 + 'px', top: i * 20 + 'px' }"
            :id="certificate.text"
          >
            <v-img :src="getImgUrl(certificate.link)" cover></v-img>
          </v-card>
        </div>
      </v-col>
    </v-row>
  </v-card>
</template>
<style scoped>
.main {
  background: rgb(207, 241, 181);
  background: linear-gradient(
    90deg,
    rgba(207, 241, 181, 1) 0%,
    rgba(173, 206, 132, 1) 46%,
    rgba(207, 241, 181, 1) 95%
  );
}
.img-container {
  position: relative;

  width: 300px;
  margin-right: 20%;
  height: 550px;
}
.img {
  position: absolute;
  height: auto;
  width: 60%;
}
.img:hover {
  z-index: 15;
}
h1 {
  font-family: "New Amsterdam", sans-serif;
  font-weight: 400;
  font-style: normal;
}
.icon {
  font-size: 150px;
  transform: rotate(-0.07turn);
  position: absolute;

  color: silver;
  opacity: 0.6;
}
</style>
