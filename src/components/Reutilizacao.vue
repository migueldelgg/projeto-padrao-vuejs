<template>
  <div>
    <button @click="ativar">Clique aqui</button>

    <span v-show="ativou">Ativado!</span>
  </div>
</template>

<script>
export default {
  nome: "Reutilizacao",
  data() {
    return {
      ativou: false,
    };
  },
  methods:{
    ativar(){
        this.ativou = !this.ativou
    }
  }
};
</script>