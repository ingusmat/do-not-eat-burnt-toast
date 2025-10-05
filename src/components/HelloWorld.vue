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
  top: -10vh;
  left: -10vh;
  z-index: -1;
  height: 110vh;
  overflow-y: hidden;
}

.big-clem img {
  height: 120vh;
  opacity: 0.8;
  object-fit: cover;
}
</style>
