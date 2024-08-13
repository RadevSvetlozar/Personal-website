<script setup>
const { size, color, top, left } = defineProps([
  "size",
  "color",
  "top",
  "left",
]);
console.log(size, color);
</script>

<template>
  <span
    class="dot"
    :style="{
      top: top + 'px',
      left: left + 'px',
      width: size + 'px',
      height: size + 'px',
    }"
  >
    <h2>dsa</h2>
    <v-icon :color="color">mdi-delete</v-icon>
    <h2>dsa</h2>
  </span>
</template>

<style scoped>
.dot {
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  position: absolute;
}
</style>
