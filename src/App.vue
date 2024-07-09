<template>
  <PrimeiroComponente />
  <LifeCycle/>
  <infoPessoa/>

</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import infoPessoa from './components/infoPessoa.vue';

export default {
  name: 'App',
  components: {
    PrimeiroComponente,
    LifeCycle,
    infoPessoa
  },
  data() {
    return {
      testando: "testando"
    }
  }
};
</script>