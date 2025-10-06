<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();
</script>

<template>
  <div class="big-clem">
    <img src="../assets/FastHappyLoudClem.png" alt="Big Clem" />
  </div>
  <div>
    <h1>{{ msg }}</h1>
  </div>
</template>

<style scoped>
.big-clem {
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  height: 100vh;
  overflow-y: hidden;
}

.big-clem img {
  height: 100vh;
  opacity: 0.8;
  object-fit: cover;
}
</style>
