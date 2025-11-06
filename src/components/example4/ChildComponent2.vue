<!-- ChildComponent.vue -->
<template>
  <div>
    <p>{{ sharedMessage }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  inject: ['sharedMessage']
});
</script>

<style scoped>
  p {
    font-size: 1.5rem;
  }
</style>
