<template>
  <div>
    <button @click="$emit('MudarImagem')">trocar imagem de perfil</button>
  </div>
</template>

<script>
export default {
  name: "MudarImagem",
  emits: ["mudarImagem"],
};
</script>