<template>
  <li class="mh-navbar__item">{{ item.text }}</li>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
});
</script>

<style lang="scss">
.mh-navbar__item {
  list-style-type: none;
}
</style>
