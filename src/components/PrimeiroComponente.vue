<template>
  <div>
    <h1>Ola vue!</h1>
    <p>Meu nome é {{ nome }} e tenho {{ age }} anos.</p>
    <p>e estudo {{ profissao }}</p>
    <MultiplosEventos/>
    <Reutilizacao/>
  </div>
</template>

<script>
import MultiplosEventos from "./MultiplosEventos.vue"
import Reutilizacao from "./Reutilizacao.vue"

export default {
  name: "PrimeiroComponente",
  components: {
    MultiplosEventos,
    Reutilizacao
  },
  data() {
    return {
      nome: "Miguel",
      age: "19",
      profissao: "desenvolvimento web.",
    };
  },
};
</script>


