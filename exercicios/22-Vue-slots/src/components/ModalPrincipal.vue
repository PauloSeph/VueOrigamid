<template>
  <div class="modal">
    <slot name="header" :alo="logo"></slot>

    <slot :user="user"></slot>

    <slot name="footer"></slot>
    
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "ModalPrincipal",
  data() {
    return {
      logo: "Batman",
      user: {
        nome: "André"
      }
    };
  }
};
</script>

<style>
</style>
