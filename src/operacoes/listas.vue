<script lang="ts">
export default {
  name: 'Lista',
}
export function itensDeLista1EstaoEmLista2(lista1: unknown[], lista2: unknown[]) {
  return lista1.every((itemLista1) => lista2.includes(itemLista1));
}
</script>

<template>

</template>

<style scoped>

</style>