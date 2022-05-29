<template>
  <nav class="mh-navbar">
    <MhNavbarItem
      v-for="item of items"
      v-bind:item="item"
      v-bind:key="item.id"
    />
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import MhNavbarItem from "./MhNavbarItem/MhNavbarItem.vue";

export default defineComponent({
  name: "MhNavbar",

  props: ["items"],

  components: { MhNavbarItem },
});
</script>

<style lang="scss">
.mh-navbar {
  display: flex;
  gap: 2vw;
}
</style>
