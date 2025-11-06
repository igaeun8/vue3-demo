<template>
  <div>
    <input v-model="id" />
    <input v-model="password" />
    <p>{{ message }}</p>
    <button @click="() => {
      this.message = this.id + ' ' + this.password;
    }">whoami</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: "E03Binding",
  data() {
    return {
      message: "Hello Vue",
      id: '',
      password: ''
    };
  }
});
</script>
