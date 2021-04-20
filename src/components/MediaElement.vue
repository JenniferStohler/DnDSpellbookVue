<template>
  <div class="media">
    <img src="//placehold.it/75x75" class="mr-3" alt="Spell" />
    <div class="media-body">
      <h5 class="mt-0">{{ spell.title }}</h5>
    </div>
  </div>
</template>

<script>
export default {
  name: "MediaElement",
  props: {
    movie: {
      type: Object,
      required: true,
    },
  },
  setup() {
    return {};
  },
  components: {},
};
</script>

<style lang="scss" scoped>
.media {
  cursor: pointer;
  &:hover {
    outline: 1px solid grey;
  }
}
</style>