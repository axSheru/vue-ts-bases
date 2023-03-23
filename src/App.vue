<script setup lang="ts">
  import { ref } from 'vue';

  const counter = ref(0);

  // Sin especificar el setup.
  /* import { defineComponent, ref } from 'vue';

  export default defineComponent({
    setup() {

      const counter = ref( 0 );

      const increment = () => {
        counter.value++;
      };

      return {
        // Properties
        counter,

        // Methods
        increment
      };

    }
  }); */

</script>

<template>
  <div class="wrapper">
    <h1>Counter: {{ counter }}</h1>
    <button @click="counter++">+1</button>
  </div>
</template>

<style scoped>
  .wrapper {
    display: flex;
    flex-direction: column;
  }
</style>
