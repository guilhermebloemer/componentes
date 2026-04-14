<script setup>
import { ref } from 'vue';
import ButtonChil from './components/ButtonChil.vue';
</script>

<template>
<div class="container">
  <div>
    <button class="btn btn-novo">Novo</button>
    <button class="btn btn-editar">Editar</button>
    <button class="btn btn-salvar">Salvar</button>
    <button class="btn btn-cancelar">Cancelar</button>
    <button class="btn btn-excluir">Excluir</button>

  </div>
  <div>
    <ButtonChil :nome="'Novo'" :tipo="'btn'" :acao="'btn-novo'">

    </ButtonChil>
  </div>
</div>
</template>

<style scoped>
. {

 justify-content: center;
}
.btn {
  color: white;
  background-color: gray;
  border-radius: 5px;
  padding: 10px 20px;
  border: none;
  cursor: crosshair;
  margin: 1px;

}

.btn-novo {
background-color: rgb(0, 223, 0);
}
.btn-editar {
background-color: rgb(38, 128, 72);
}
.btn-salvar {
background-color: rgb(221, 207, 6);
}
.btn-cancelar{
background-color: rgb(235, 113, 0);
}
.btn-excluir {
background-color: rgb(253, 8, 8);
}


</style>
