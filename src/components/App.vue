<template>
  <button @click="plusCount">{{ count }}</button>
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
});
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;

  body {
    color: red;
  }
}
</style>
