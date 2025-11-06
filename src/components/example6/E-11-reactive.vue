<template>
  <div>
    <p>Name: {{ person.name }}</p>
    <p>Age: {{ person.age }}</p>
    <button @click="incrementAge">Increment Age</button>
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive } from 'vue';

export default defineComponent({
  name: 'E11Reactive',
  setup() {
    const person = reactive({
      name: 'John Doe',
      age: 30
    });

    const incrementAge = () => {
      person.age++; // reactive는 바로 속성에 접근
    };

    return {
      person,
      incrementAge
    };
  }
});
</script>
