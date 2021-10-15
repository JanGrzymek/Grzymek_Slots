<template>
  <div class="layout">
    <header class="header"><slot name="header"></slot></header>
    <main><slot></slot></main>
    <footer class="footer"><slot name="footer"></slot></footer>
  </div>
</template>
<style>
.header {
  background-color: lightgreen;
}
.footer {
  background-color: lightgreen;
}
</style>
