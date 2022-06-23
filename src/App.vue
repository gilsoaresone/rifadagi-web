<template >


    <div class="conteiner" >
      <Topo />
      <cadastrar /><br>
      <buscar />
    </div>
  


</template>

<script>
import cadastrar from "./components/Cadastrar.vue"
import Buscar from "./components/Buscar.vue"
import Topo from "./components/Topo.vue"
export default {

  components: {
    cadastrar,
    Buscar,
    Topo
  }
}
</script>

<style scoped>
.conteiner {

margin: 5px;

}
</style>>

