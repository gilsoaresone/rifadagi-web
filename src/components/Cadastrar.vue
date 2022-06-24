<template>
    <div id="cadastrar">
  <b-row class="my-1">
    <b-col sm="2">
      <label for="input-small">Nome:</label>
    </b-col>
    <b-col sm="10">
      <b-form-input  size="sm" v-model="nome" placeholder="Digite o seu nome "></b-form-input>
    </b-col>
  </b-row>
  <b-row class="my-1">
    <b-col sm="2">
      <label >Numero:</label>
    </b-col>
    <b-col sm="10">
      <b-form-input  size="sm" v-model="numero" placeholder="Digite um numero disponivel de 1 a 100"></b-form-input>
    </b-col>
  </b-row>
<div><b-button variant="outline-dark" @click="postar(), reloadPage() ">Cadastrar</b-button>

</div>



      
    </div>
</template>
<script>
import axios from "axios"
export default {
    name: 'cadastrarRifa',
    data() {
        return {
            resultado: [],
            nome: "",
            numero: "",
        }
    },
    methods: {
      async  postar() {
          await  axios.post("https://rifagi.herokuapp.com/api/rifa",
                {
                    numero: this.numero,
                    nome: this.nome
                }
            )
        },

        
         reloadPage() {
 setInterval('window.location.reload()', 1000);
    
    }

    },
  
}
</script>


