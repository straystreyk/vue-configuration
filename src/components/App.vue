<template>
  <div>
    Hello vue
    <button @click="plusCount">{{ plusFormatter }}</button>
    <router-view />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  data() {
    return {
      count: 101,
    };
  },
  methods: {
    plusCount() {
      this.count += 1;
    },
  },
  computed: {
    plusFormatter() {
      return this.count;
    },
  },
});
</script>

<style lang="scss">
@import "./index";
</style>
