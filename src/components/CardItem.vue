<template>
  <section class="card">
    <header @click="toggleAccordion()" class="card-header">
      <i>
        <slot name="icon"></slot>
      </i>
      <h2><slot name="title"></slot></h2>
    </header>
    <div v-show="isOpen" class="card-body">
      <slot name="contents"></slot>
    </div>
    <footer v-show="isOpen" class="card-footer">
      <cite>Credit: <slot name="author"></slot></cite>
    </footer>
  </section>
</template>

<script lang="ts">
export default {
  props: ["title"],
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggleAccordion() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>

<style scoped>
.card {
  width: 750px;
  margin-bottom: 40px;
  border-radius: 6px;
  /* background-color: #141e32; */
  background-color: var(--color-background-mute);
  grid-column: 1;
}

.card-header {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  padding: 8px 16px;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  border-bottom-style: solid;
  border-bottom-width: 1px;
  border-color: var(--color-border);
  background-color: var(--color-background-soft);
  color: #0ac8ff;
  cursor: pointer;
}

.card-body {
  width: 100%;
  color: white;
  padding: 16px;
}

.card-footer {
  padding: 8px 16px;
  border-top-style: solid;
  border-top-width: 1px;
  border-color: var(--color-border);
  background-color: var(--color-background-soft);
}

/* .show-btn {
  margin-left: 2px;
  color: #0ac8ff;
  background-color: #141e32;
  border: none;
  cursor: pointer;
} */
</style>

<!-- <script lang="ts">
export default {
  props: ["title"],
  data() {
    return {
      show: true,
    };
  },
};
</script>

<template>
  <section class="card">
    <header class="card-header">
      <i>
        <slot name="icon"></slot>
      </i>
      <h2>
        {{ title }}
      </h2>
      <button @click="show = !show" class="show-btn">Toggle</button>
    </header>
    <div v-if="show" class="card-body">
      <slot name="contents"></slot>
    </div>
    <footer class="card-footer">Credit to <slot name="author"></slot></footer>
  </section>
</template>

<style scoped>
.card {
  margin-bottom: 40px;
  border-radius: 6px;
  background-color: #141e32;
  grid-column: 1;
}
.card-header {
  color: #0ac8ff;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  padding: 8px 16px;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
  border-bottom-style: solid;
  border-bottom-width: 1px;
}

.card-body {
  color: white;
  padding: 16px;
}

.card-footer {
  padding: 8px 16px;
}
.show-btn {
  margin-left: 2px;
}
</style> -->
