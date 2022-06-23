<template>
  <div class="conteiner">
    <Topo/>
    <cadastrar/>
    <buscar/>
  </div>

</template>

<script>
import cadastrar from "./components/Cadastrar.vue"
import Buscar from "./components/Buscar.vue"
import Topo from "./components/Topo.vue"
export default {
 
 components:{
  cadastrar,
  Buscar,
  Topo
 }
}
</script>

<style scoped>
.conteiner{
 width: 1200px;
 margin: auto;
 margin-top: 50px;

}
</style>>

