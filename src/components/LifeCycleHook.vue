<template>
  <h6>Meu nome é: {{ nome }}</h6>
</template>

<script>
export default {
  nome: "LifeCycle",
  data() {
    return {
      nome: "ainda nao definido",
    };
  },
  // Posso mudar o componente de acordo com eventos
  //quando o componente for criado ele exibe isso
  created() {
    setTimeout(() => {
      this.nome = "Eliezer";
    }, 1000);
  },
  //quando o componente for montado exibe isso
  mounted() {
    setTimeout(() => {
      this.nome = "Thalissa";
    }, 2000);
  },
};
</script>