<script lang="ts">

import {defineComponent} from "vue";
import Banner from "@/components/Banner.vue";
import ConteudoPrincipal from "@/components/ConteudoPrincipal.vue";

export default defineComponent({
  components: {ConteudoPrincipal, Banner}
})
</script>

<template>
  <Banner/>
  <ConteudoPrincipal/>
</template>


<style scoped>

</style>
