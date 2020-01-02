<template>
  <div id="app">
    <modal-principal>

       <template #header="{alo}">
        <p>Esse é o Header</p>
        <p>{{alo}}</p>
      </template>

      <template #default="{user}">
        <p>Conteudo default</p>
        <button>Comprar</button>
        {{user.nome}}
      </template>

      <template #footer>
        <p>Esse é o Footer</p>
      </template>
    </modal-principal>

  </div>
</template>

<script>
import ModalPrincipal from "./components/ModalPrincipal.vue";


export default {
  name: "app",
  components: {
    ModalPrincipal


  }
};
</script>

<style>
</style>
