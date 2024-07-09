<template> 
  <div>
    <h1> Ola vue!</h1>
    <p>Meu nome é {{ nome }} e tenho {{ age }} anos.</p>
    <p>e estudo {{ profissao }}</p>
  </div>
</template>

<script>
export default {
  name: 'PrimeiroComponente',
  data() {
    return {
      nome: "Miguel",
      age: "19",
      profissao: "desenvolvimento web."
    }
  }
};
</script>


