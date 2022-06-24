<template >


    <div class="conteiner" >

      
     
      <Topo />


<Premio/>
<br>
      <cadastrar /><br>
      <buscar />

   
    </div>
  


</template>

<script>

import Premio from "./components/Premio.vue"
import cadastrar from "./components/Cadastrar.vue"
import Buscar from "./components/Buscar.vue"
import Topo from "./components/Topo.vue"
export default {

  components: {
    cadastrar,
    Buscar,
    Topo,
    Premio
  }
}
</script>

<style scoped>
.conteiner {

margin: 5px;

}
</style>>

