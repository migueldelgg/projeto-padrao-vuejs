<template>
  <Header/>
  <Form/>
  <PrimeiroComponente />
  <LifeCycle />
  <infoPessoa />
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import infoPessoa from "./components/infoPessoa.vue";
import Header from "./components/Header.vue"
import Form from "./components/Form.vue"

export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    infoPessoa,
    Header,
    Form
  },
  data() {
    return {
      testando: "testando",
    };
  },
};
</script>

<style>

  body {
    background-color: #0D1117;
    color: aliceblue;
  }

  a {
    color: blue;
  }
  .teste{
    background-color: white;
    color:#0D1117;
  }
</style>