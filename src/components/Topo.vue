<template>
   <div class="topo">
   <span class="titulo"> Rifa da gi</span><br><span class="valor">Valor R$10,00</span> <br><span class="pix">Pix 11 981627125</span><br>
   <span class="contato">Contatos: 11 98162-7125 | 11 98677-1371 </span>
    <br>  <br>
    <p class="cupom">*Cupom válido de segunda à sexta feira das 9h às 21h. Marcado com antecedência</p>
    
   </div>
</template>

<script>
export default {
    name:'topRifa',
    data(){
        return{

        }
    }
    
}
</script>

<style>

.titulo{
    color: #80411f;
    font-size: 36px;
}
.valor{
    font-size: 18px;
       color: #552811;
}
.pix{
    font-weight: bold;
    font-size: 14px;
     color: #964d28;
}
.contato{
      
    font-size: 14px;
       color: #80411f;
}
.cupom{
      color: #80411f;
    font-weight: bolder;
       font-size: 10px;
}
</style>