<script setup>
import HOME from './components/Home.vue'
import FOOTER from './components/footer.vue'
import BUTTON from "./components/Button.vue"
</script>

<template>
  <div>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/uphasia_logo.png" class="logo" alt="Vue logo" />
    </a>
  </div>
  <HOME/>
  <BUTTON/>
  <FOOTER/>
</template>

<style scoped>
.logo {
  height: 7em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}

</style>
