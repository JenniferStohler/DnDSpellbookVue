<template>
  <div class="Results">
    <!-- NOTE to pass prop data to a child component it is passed as a bound attribute -->
    <MediaElement
      v-for="spell in state.results"
      :key="spell.id"
      :spell="spell"
      @click="setActive(spell)"
    />
  </div>
</template>

<script>
import { computed, reactive } from "vue";
import { AppState } from "../AppState";
import { spellsService } from "../services/SpellsService";
import MediaElement from "./MediaElementComponent";
export default {
  name: "results",
  setup() {
    const state = reactive({
      results: computed(() => AppState.results),
    });
    return {
      state,
      setActive(spell) {
        spellsService.setActive(spell);
      },
    };
  },
  components: {
    MediaElement,
  },
};
</script>

<style lang="scss" scoped>