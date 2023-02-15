<script setup lang="ts">
import TheWelcome from "../components/TheWelcome.vue";
import TheTips from "@/components/TheTips.vue";
// import TheSideNav from "@/components/TheSideNav.vue";
</script>

<template>
  <main>
    <TheTips />
  </main>
</template>

<style scoped>
main {
  grid-column-start: 1;
  grid-column-end: 2;
  grid-row-start: 3;
  grid-row-end: 3;
}
</style>
