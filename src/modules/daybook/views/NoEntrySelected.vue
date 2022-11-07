<template>
  <div class="d-flex justify-content-center">
        <h1 class="align-self-center text-center">No hay  nada seleccionado</h1>
  </div>
  <FabN></FabN>
</template>

<script>

import  {defineAsyncComponent} from "vue";

export default {
    components:{
      FabN: defineAsyncComponent(() => import('../components/FabN.vue'))
    }
}
</script>

<style lang="scss" scoped>

div{
    height: 100%;
}

</style>