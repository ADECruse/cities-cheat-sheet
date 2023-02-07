<template>
  <section class="card">
    <header class="card-header">
      <i>
        <slot name="icon"></slot>
      </i>
      <h2>
        <slot name="heading"></slot>
      </h2>
    </header>
    <div class="card-body">
      <slot></slot>
    </div>
  </section>
</template>

<style scoped>
.card {
  margin-bottom: 40px;
  border-radius: 6px;
  background-color: #141E32;
  grid-column: 1;
}
.card-header {
color: #0AC8FF;
  text-align: start;
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
</style>
