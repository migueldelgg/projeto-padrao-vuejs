<template>
  <Header :esta_logado="true"/>
  <Form />
  <PrimeiroComponente />
  <LifeCycle />
  <infoPessoa :email="email" :esta_trabalhando=false />
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import infoPessoa from "./components/infoPessoa.vue";
import Header from "./components/Header.vue";
import Form from "./components/Form.vue";

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
      email: "miguel.delg2004@gmail.com"
    };
  }
};
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

  body {
    background-color: #0D1117;
    color: aliceblue;
    font-family: 'Roboto', sans-serif; /* Altera a fonte de todos os textos */
  }

  a {
    color: #1034A8;
  }

  .teste {
    background-color: white;
    color: #0D1117;
  }
</style>
