<template>
  <PrimeiroComponente />
  <p>O dado do componente app é {{ testando }}</p>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';

export default {
  name: 'App',
  components: {
    PrimeiroComponente
  },
  data() {
    return {
      testando: "testando"
    }
  }
};
</script>
