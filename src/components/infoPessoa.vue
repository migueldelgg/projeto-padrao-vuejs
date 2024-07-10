<template>
  <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
  <p v-else>estou em busca de novas oportunidades</p>

  <p>Utilizo as seguintes tecnologias:</p>
  <ul>
    <li>JavaScript</li>
    <li>PHP</li>
    <li>Python</li>
  </ul>
  <p class="teste">
    para acessar meu portifolio basta clicar<a v-bind:href="meu_link" target="_blank"> aqui</a>
  </p>
  <div>
    <button @click="showEmail">{{textoBotao}}</button>
    <p v-show="mostrar_email">Manda uma mensagem para: {{ email }}</p>
  </div>
  <Picture/>
</template>
<script>

import Picture from './Picture.vue'

export default {
  name: "Info",
  data() {
    return {
      email: "miguel.delg2004@gmail.com",
      esta_trabalhando: false,
      mostrar_email: false,
      meu_link: "https://github.com/migueldelgg",
      textoBotao: 'Mostrar e-mail'
    };
  },
  components: {
    Picture
  },
  methods: {
    showEmail(){
      this.mostrar_email = !this.mostrar_email
      if(this.mostrar_email == false){
        this.textoBotao = 'Mostrar e-mail'
      }else {
        this.textoBotao = 'Esconder e-mail'
      }
    }
  }
};
</script>
