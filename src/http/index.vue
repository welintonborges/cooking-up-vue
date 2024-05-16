<script lang="ts">

import ICategoria from "@/interfaces/ICategoria.vue";
import IReceita from "@/interfaces/IReceita.vue";

// export async function obterCategoria() {
//   // const resposta = await fetch('https://gist.githubusercontent.com/antonio-evaldo/002ad55e1cf01ef3fc6ee4feb9152964/raw/07e853b7d0626db51ce2e84bb2f15ca450b7bd7f/categorias.json')
//   // const categorias:ICategoria = await resposta.json();
//   // return categorias;
//
//   // await new Promise((resolver) => {
//   //   setTimeout(resolver, 3000);
//   // })
// }
  async function obterDadosURL<T>(url: string) {
    const resposta = await fetch(url);
    return resposta.json() as T;
  }

  export async function obterCategorias() {
    return obterDadosURL<ICategoria[]>('https://gist.githubusercontent.com/antonio-evaldo/002ad55e1cf01ef3fc6ee4feb9152964/raw/bf463b47860043da3b3604ca60cffc3ad1ba9865/categorias.json');
  }

  export async function obterReceitas() {
    return obterDadosURL<IReceita[]>('https://gist.githubusercontent.com/antonio-evaldo/002ad55e1cf01ef3fc6ee4feb9152964/raw/bf463b47860043da3b3604ca60cffc3ad1ba9865/receitas.json');
  }



</script>

<template>

</template>

<style scoped>

</style>