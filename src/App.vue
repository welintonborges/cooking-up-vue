<script lang="ts">

import {defineComponent} from "vue";
import Banner from "@/components/Banner.vue";
import ConteudoPrincipal from "@/components/ConteudoPrincipal.vue";
import Rodape from "@/components/Rodape.vue";

export default defineComponent({
  components: {Rodape, ConteudoPrincipal, Banner}
})
</script>

<template>
  <Banner/>
  <ConteudoPrincipal/>
  <Rodape/>
</template>


<style scoped>

</style>
