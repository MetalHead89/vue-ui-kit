<template>
  <header class="mh-header">
    <img src="" alt="" />
    <mh-navbar :items="items" />
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import MhNavbar from "@/components/MhNavbar/MhNavbar.vue";

export default defineComponent({
  components: {
    MhNavbar,
  },

  props: ["items"],
});
</script>

<style lang="scss">
$padding: 2vw;

.mh-header {
  box-sizing: border-box;
  display: flex;
  justify-content: space-between;
  width: 100%;
  padding: $padding;
  border: 1px solid black;
}
</style>
