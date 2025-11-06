<template>
  <div>Hello, {{ message }}</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: "E01Instance",
  data() {

    const name = 'Gaeun Lee'

    return {
      message: name,
    };
  }
});
</script>

<style scoped>
div {
  color: blue;
  font-size: 20px;
  font-weight: bold;
}
</style>
