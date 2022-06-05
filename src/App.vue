<template>
  <div class="app__simple-components">
    <section class="app__component">
      <h2 class="app__component-title">Navbar</h2>
      <mh-navbar v-bind:items="items" />
    </section>
  </div>
  <section class="app__component">
    <div class="app__title-container">
      <h2 class="app__component-title">Header</h2>
    </div>
    <mh-header v-bind:items="items" />
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import MhNavbar from "@/components/MhNavbar/MhNavbar.vue";
import MhHeader from "@/components/MhHeader/MhHeader.vue";

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
    MhHeader,
  },
});
</script>

<style lang="scss">
.app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

  &__simple-components {
    padding: 0 1vw;
  }

  &__component {
    padding: 1vw 0;
  }

  &__title-container {
    padding: 0 1vw;
  }

  &__component-title {
    size: 3vw;
    text-align: left;
  }
}
</style>
