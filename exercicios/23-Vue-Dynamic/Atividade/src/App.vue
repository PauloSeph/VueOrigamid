<template>
  <div id="app">
    <ul>
      <li @click="abaAtiva = 'SobreEmpresa'">Sobre</li>
      <li @click="abaAtiva = 'ServicosEmpresa'">Servicos</li>
      <li @click="abaAtiva = 'ContatoEmpresa'">Contato</li>
    </ul>
    <keep-alive>
    <component :is="abaAtiva"></component>
    </keep-alive>
  </div>
</template>

<script>
import SobreEmpresa from "./components/SobreEmpresa";
import ContatoEmpresa from "./components/ContatoEmpresa";
import ServicosEmpresa from "./components/ServicosEmpresa.vue";

export default {
  name: "app",
  components: {
    SobreEmpresa,
    ContatoEmpresa,
    ServicosEmpresa
  },
  data() {
    return {
      abaAtiva: ""
    }
  }
}
</script>

<style>

</style>