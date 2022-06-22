<template>
  <div id="app">
   <ul v-for="result in resultado" :key="result._id">
    <li v-bind:disabled="result._id === result._id ? true : false">Protocolo:  v-for="result in resultado" :key="result._id"</li>
    <li>Data agendada: {{result.dataAgendada}}</li>
   </ul>




    <button @click="pegar()">carregar</button>
  </div>
</template>

<script>

import axios from "axios"

export default {
  name: 'App',
data(){
  return{
resultado:[]
  }
},
  methods:{
    pegar(){
      axios.get("https://certificadodigital.herokuapp.com/api/agendamento")
      .then((res)=>{
        this.resultado = res.data
        console.log(res.data)
        
        
      }).catch((error)=>{
        console.log(error)
      })
    }
  }
}
</script>


