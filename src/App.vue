<template>
  <MhNavbar v-bind:items="items" />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import MhNavbar from "@/components/MhNavbar/MhNavbar.vue";

export default defineComponent({
  name: "App",

  data() {
    return {
      items: [
        { id: 1, text: "item 1" },
        { id: 2, text: "item 2" },
        { id: 3, text: "item 3" },
        { id: 4, text: "item 4" },
        { id: 5, text: "item 5" },
      ],
    };
  },

  components: {
    MhNavbar,
  },
});
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
