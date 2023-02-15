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

    <template v-for="card in cards">
      <a>{{ card.title }}</a>
    </template>
  </nav>
</template>
<style scoped>
#sidemenu {
  display: flex;
  min-width: 300px;
  /* grid-column-start: 2;
  grid-row-start: 1;
  grid-row-end: 2; */
  flex: auto;
  flex-direction: column;
  position: fixed;
  z-index: 1;
  top: 0;
  right: 0;

  
}

#sidemenu a {
  padding: 7px 8px 7px 32px;
}

.btn-group {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.btn-side-nav {
  background-color: var(--color-background-mute);
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  font-size: 16px;
  border-radius: 6px;
  cursor: pointer;
}

.btn-side-nav:hover {
  background-color: var(--color-background-soft);
}
</style>
