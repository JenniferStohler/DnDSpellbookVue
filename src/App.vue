<template>
  <h1>
    <img class="img-logo" alt="Vue logo" src="./assets/logo.png" />Your DnD
    Spellbook
  </h1>
  <HomePage />
</template>

<script>
import HomePage from "./pages/HomePage.vue";
export default {
  name: "App",
  components: {
    HomePage,
  },
};
</script>

<style lang="scss">
@import "./assets/main.scss" .img-logo {
  height: 0.75em;
}
h1 {
  color: rgb(5, 5, 5);
}
</style>
