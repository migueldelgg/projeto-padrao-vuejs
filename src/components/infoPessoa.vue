<template>

  <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
  <p v-else>estou em busca de novas oportunidades</p>

  <p>Utilizo as seguintes tecnologias:</p>
  <ul>
    <li>JavaScript</li>
    <li>PHP</li>
    <li>Python</li>
  </ul>
  <p v-show="mostrar_email">Manda uma mensagem para: {{ email }}</p>
</template>
<script>
export default {
  name: "Info",
  data(){
    return {
      email: "miguel.delg2004@gmail.com",
      esta_trabalhando: false,
      mostrar_email: true
    }
  }
};
</script>
