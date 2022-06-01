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
$color: #414141;
$hovered-color: #797979;
$size: 1vw;
$weight: 800;

.mh-navbar__item {
  color: $color;
  font-size: $size;
  font-weight: $weight;
  list-style-type: none;
  cursor: pointer;

  &:hover {
    color: $hovered-color;
  }
}
</style>
