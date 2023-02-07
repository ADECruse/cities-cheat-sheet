<script setup lang="ts">
import TheWelcome from "../components/TheWelcome.vue";
import TheTips from "@/components/TheTips.vue";
</script>

<template>
  <main>
    <TheTips />
  </main>
</template>

<style scoped >
main {
  grid-column-start: 1;
  grid-row-start: 2;
}
</style>