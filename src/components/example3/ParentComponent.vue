<!-- ParentComponent.vue -->
<template>
  <div>
    <ChildComponent
        :message="parentMessage"
        :id="1"
        :password="1234"
        @custom-event="handleEvent"
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ChildComponent from './ChildComponent.vue';

export default defineComponent({
  name: "E05ParentComponent",
  data() {
    return {
      parentMessage: 'Hello from parent'
    };
  },
  methods: {
    handleEvent(payload: any) {
      console.log(payload);
    }
  },
  components: {
    ChildComponent
  }
});
</script>
