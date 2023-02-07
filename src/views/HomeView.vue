<script setup lang="ts">
import TheWelcome from "../components/TheWelcome.vue";
import TheTips from "@/components/TheTips.vue";
import SideNav from "@/components/SideNav.vue";
</script>

<template>
  <main>
    
    <TheTips />
  </main>
  <SideNav />
</template>

<style scoped >
main {
  grid-column-start: 1;
  grid-row-start: 2;
}
</style>