<script lang="ts">
export default {
  data() {
    return {
      isExpanded: true,
    };
  },
  props: {
    cards: Array,
  },

  methods: {
    collapseAll() {},
    expandAll() {},
  },
};
</script>
<template>
  <nav id="sidemenu">
    <div class="btn-group">
      <button @click="collapseAll" class="btn-side-nav">Collapse All</button>
      <button @click="expandAll" class="btn-side-nav">Expand All</button>
    </div>

    <template v-for="card in cards" :key="card.id">
      <a>{{ card.title }}</a>
    </template>
  </nav>
</template>
<style scoped>
#sidemenu {
  display: flex;
  min-width: 300px;
  height: 100%;
  flex: auto;
  flex-direction: column;
  position: fixed;
  z-index: 1;
  top: 0;
  right: 0;
  background-color: black;
}

#sidemenu a {
  padding: 7px 8px 7px 32px;
}

.btn-group {
  display: flex;
  flex-direction: row;
  justify-content: center;
  padding: 6px;
}

.btn-side-nav {
  background-color: var(--color-background-mute);
  border: none;
  color: white;
  padding: 10px 30px;
  text-align: center;
  text-decoration: none;
  font-size: 16px;
  border-radius: 6px;
  cursor: pointer;
  margin: 2px;
}

.btn-side-nav:hover {
  background-color: var(--color-background-soft);
}
</style>
