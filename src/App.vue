<template>
  <div class="container mt-5">
    <h1>Arithmetic Calculator</h1>
    <calculator></calculator>
  </div>
</template>

<script>
import Calculator from './components/Calculator.vue';

export default {
  components: {
    Calculator,
  },
};
</script>