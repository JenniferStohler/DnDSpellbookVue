<template>
  <div>
    <h1>
      <img class="img-logo" alt="Vue logo" src="./assets/logo.png" />Your DnD
      Spellbook
    </h1>
    <HomePage />
  </div>
</template>

<script>
import HomePage from "./components/HomePage";
export default {
  name: "App",
  components: {
    HomePage,
  },
};
</script>

<style lang="scss">
</style>
