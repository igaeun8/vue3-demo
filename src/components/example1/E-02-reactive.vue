<template>
  <div>{{ fullName }}</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

interface Data {
  firstName: string;
  lastName: string;
}

export default defineComponent({
  name: "E02Reactive",
  data(): Data {
    return {
      firstName: "Gaeun",
      lastName: "Lee"
    };
  },
  mounted() {

    console.log('mounted');

    let a = 10;

    setTimeout(() => {
      console.log('setTimeout');
      a = 20;
      console.log(a);
    }, 500);

    setTimeout(() => {
      this.lastName = "123";
    }, 1000);

    setTimeout(() => {
      this.firstName = "LGE";
    }, 2000);
  },
  computed: {
    fullName(): string {
      return this.firstName + " " + this.lastName;
    }
  }
});
</script>
