<script setup></script>

<template>
  <v-card id="education">
    <v-card
      elevation="23"
      color="transparent"
      style="margin: auto"
      width="800px"
        max-height="700px"
      height="100vh"
    >
      <svg width="100%" height="850px">
        <line x1="280" y1="50" x2="550" y2="100" stroke="black" />
        <line x1="450" y1="350" x2="550" y2="100" stroke="black" />
        <line x1="300" y1="280" x2="450" y2="300" stroke="black" />
        <line x1="100" y1="350" x2="250" y2="250" stroke="black" />
        <line x1="100" y1="350" x2="450" y2="450" stroke="black" />
        <line x1="700" y1="500" x2="450" y2="480" stroke="black" />
        <line x1="700" y1="500" x2="500" y2="680" stroke="black" />
        <line x1="220" y1="680" x2="500" y2="680" stroke="black" />
      </svg>

      <span class="dot born">
        <h3>Born</h3>
        <v-icon color="green">mdi-baby</v-icon>
        <h4>1994</h4>
      </span>

      <span class="dot basic">
        <h3>Primary</h3>
        <h3>Education</h3>
        <v-icon color="yellow">mdi-book-open-blank-variant-outline</v-icon>
        <h4>2004</h4>
      </span>

      <span class="dot average">
        <h3>Higher</h3>
        <h3>Education</h3>
        <v-icon color="purple">mdi-cast-education</v-icon>
        <h4>2013</h4>
      </span>

      <span class="dot electrican">
        <h3>Electrican</h3>
        <v-icon color="blue">mdi-lightning-bolt</v-icon>
        <h4>2016</h4>
      </span>
      <span class="dot substation">
        <h3>Power</h3>
        <h3>Substation</h3>
        <h3>Operator</h3>
        <v-icon color="red">mdi-transmission-tower</v-icon>
        <h4>2018</h4>
      </span>

      <span class="dot master">
        <h3>Master</h3>
        <h3>Electrical</h3>
        <h3>Engineer</h3>
        <v-icon color="lime">mdi-account-hard-hat</v-icon>
        <h4>2019</h4>
      </span>
      <span class="dot back">
        <h3>Back-End</h3>
        <h3>Dev C#</h3>
        <v-icon color="red">mdi-code-greater-than-or-equal</v-icon>
        <h4>2020</h4>
      </span>
      <span class="dot end">
        <h3>Front-End</h3>
        <h3>Dev VueJS</h3>
        <v-icon color="cyan">mdi-google-chrome</v-icon>
        <h4>2022</h4>
      </span>
      <span class="dot now">
        <h3>Full-Stack</h3>
        <h3>Dev</h3>
        <v-icon color="orange">mdi-xml</v-icon>
        <h4>Nowadays</h4>
      </span>
    </v-card>
    <div
      class="left-bar"
      style="background-color: white; width: 150px; top: 400px"
    ></div>
    <div
      class="left-bar"
      style="background-color: #cdf7cd; width: 250px; top: 490px"
    ></div>
    <div
      class="left-bar"
      style="background-color: #8c705a; width: 170px; top: 560px"
    ></div>
    <div
      class="right-bar"
      style="background-color: #cdf7cd; width: 230px; top: 130px"
    ></div>
    <div
      class="right-bar"
      style="background-color: #8c705a; width: 200px; top: 230px"
    ></div>
    <div
      class="right-bar"
      style="background-color: white; width: 170px; top: 330px"
    ></div>
  </v-card>
</template>

<style scoped>
.right-bar {
  position: absolute;
  right: -50px;
  height: 30px;
  border-radius: 20px;
  transform: rotate(0.1turn);
  opacity: 0.6;
  -webkit-box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
  box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
}
.left-bar {
  position: absolute;
  left: -50px;
  height: 30px;
  border-radius: 20px;
  transform: rotate(0.1turn);
  opacity: 0.85;
  -webkit-box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
  box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
}
.now {
  top: 650px;
  left: 150px;
  height: 180px;
  width: 180px;
}
.end {
  top: 590px;
  left: 480px;
  height: 160px;
  width: 160px;
}
.back {
  top: 450px;
  left: 650px;
  height: 140px;
  width: 140px;
}
.master {
  top: 410px;
  left: 350px;
  height: 160px;
  width: 160px;
}
.substation {
  top: 300px;
  left: 50px;
  height: 140px;
  width: 140px;
}
.electrican {
  top: 200px;
  left: 200px;
  height: 120px;
  width: 120px;
}
.average {
  top: 240px;
  left: 400px;
  height: 120px;
  width: 120px;
}
.basic {
  top: 70px;
  left: 500px;
  height: 120px;
  width: 120px;
}
.born {
  top: 20px;
  left: 200px;
  height: 100px;
  width: 100px;
}

.dot {
  background-color: white;
  border-radius: 50%;
  border: 2px dashed silver;
  display: inline-block;
  position: absolute;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  -webkit-box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
  box-shadow: 10px 10px 86px 0px rgba(0, 0, 0, 0.75);
}
h2 {
  color: white;
}
</style>
