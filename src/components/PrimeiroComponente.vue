<template>
  <div>
    <h6>Meu nome é: {{ nome }}</h6>
  </div>
</template>

<script>
// Exportando um componente passando o nome dele
export default {
  name: "PrimeiroComponente",
  data() {
    return {
      nome: "Eliézer",
    };
  },
};
</script>