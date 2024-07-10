<template>
  <h1>meu nome é: {{ nome }}</h1>
</template>

<script>
export default {
  name: "LifeCycle",
  data() {
    return {
      nome: "Ainda nao sei",
    };
  },
  created() {
    setTimeout(() => {
      this.nome = "Julio";
    }, 1000);
    this.lifeCycle();
  },
  mounted() {
    setTimeout(() => {
      this.nome = "Pedro";
    }, 2000);
    this.lifeCycle();
  },
  methods: {
    lifeCycle() {
      console.log("executou");
    },
  },
};
</script>