<!-- ParentComponent.vue -->
<template>
  <div>
    <ChildComponent1 />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ChildComponent1 from "@/components/example4/ChildComponent1.vue";

export default defineComponent({
  name: "E06ParentComponent",
  provide() {
    return {
      sharedMessage: 'Hello from provide'
    };
  },
  components: {
    ChildComponent1
  }
});
</script>
