<template>
  <div id="buscar">
      <div>
     <b-table sort-by="numero" sortDesc striped hover :items="resultado" :fields="fields" ></b-table>
  </div>

  </div>
</template>

<script>

import axios from "axios"


export default {
  name: 'buscarRifa',
data(){
  return{
     fields: ['nome', 'numero'],
resultado:[],
nome: "",
numero:"",

  }
},




  created (){
  axios.get("https://rifagi.herokuapp.com/api/rifa")
      .then((res)=>{
        this.resultado = res.data
      
        console.log(res.data)
        
        
      }).catch((error)=>{
        console.log(error)
      })

  },
}
</script>