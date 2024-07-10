<template>
    <div>
      <h1>Formulário Simples</h1>
      <form @submit.prevent="handleSubmit">
        <div>
          <label for="name">Nome:</label>
          <input type="text" id="name" v-model="formData.name" required />
        </div>
        <div>
          <label for="email">E-mail:</label>
          <input type="email" id="email" v-model="formData.email" required />
        </div>
        <div>
          <label for="message">Mensagem:</label>
          <textarea id="message" v-model="formData.message" required></textarea>
        </div>
        <button type="submit">Enviar</button>
      </form>
  
      <div v-if="submitted">
        <h2>Dados Enviados:</h2>
        <p><strong>Nome:</strong> {{ formData.name }}</p>
        <p><strong>E-mail:</strong> {{ formData.email }}</p>
        <p><strong>Mensagem:</strong> {{ formData.message }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        formData: {
          name: '',
          email: '',
          message: ''
        },
        submitted: false
      };
    },
    methods: {
      handleSubmit() {
        this.submitted = true;
        // Aqui você pode adicionar lógica para enviar os dados para um servidor, se necessário
        console.log('Dados do formulário:', this.formData);
      }
    }
  };
  </script>
  
  <style scoped>
  form {
    max-width: 500px;
    margin: 0 auto;
  }
  
  div {
    margin-bottom: 1em;
  }
  
  label {
    display: block;
    margin-bottom: 0.5em;
  }
  
  input,
  textarea {
    width: 100%;
    padding: 0.5em;
    margin-bottom: 0.5em;
  }
  
  button {
    padding: 0.5em 1em;
    background-color: #42b983;
    color: white;
    border: none;
    cursor: pointer;
  }
  
  button:hover {
    background-color: #38a169;
  }
  </style>
  