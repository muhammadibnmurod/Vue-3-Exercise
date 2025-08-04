<script setup lang="ts">

</script>

<template>
  <div class="wrapper">
    <aside class="sibebar">
    <slot name="sidebar" />
    </aside>
    <main>
    <slot name="main" />
    </main>
  </div>
  <footer>
  <slot name="footer" />
  </footer>
</template>

<style scoped>
 .sibebar {
   border: 2px solid green;
 }
 .main {
   border: 2px solid blue;
 }
 .footer {
   border: 2px solid red;
 }
</style>
