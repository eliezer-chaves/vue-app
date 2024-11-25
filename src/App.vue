<template>
  <div>
    <h3>
      Esse componente é do App: {{ local }}
    </h3>   
    <h3>
      Esse componente é do Primeiro Componente: <PrimeiroComponente/>
    </h3>     
    <h3>
      Essa tag é do: <life-cycle-hook/>
    </h3>
  </div>
</template>

<script>
//trazendo para o app o componente
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycleHook from "./components/LifeCycleHook.vue";

//Exportando o componente App e o PrimeiroComponente
export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycleHook,
  },
  data() {
    return {
      local: "Componente App",
    };
  },
};
</script>