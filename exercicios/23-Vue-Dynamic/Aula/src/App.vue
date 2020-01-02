<template>
  <div id="app">
    <button @click="componenteAtivo = 'AulaDescricao'">Descrição</button>
    <button @click="componenteAtivo = 'AulaDonwload'">Donwload</button>
    <keep-alive>
    <component :is="componenteAtivo"></component>
    </keep-alive>
  </div>
</template>

<script>
import AulaDescricao from "./components/AulaDescricao.vue";
import AulaDonwload from "./components/AulaDonwload.vue";

export default {
  name: "app",
  components: {
    AulaDescricao,
    AulaDonwload
  },
  data() {
    return {
      componenteAtivo: ""
    }
  }
}
</script>

<style>

</style>