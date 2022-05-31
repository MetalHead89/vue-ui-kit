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
  color: #414141;
  font-size: 1vw;
  font-weight: 800;
  list-style-type: none;
  cursor: pointer;

  &:hover {
    color: #797979;
  }
}
</style>
