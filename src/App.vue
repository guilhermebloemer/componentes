<script setup>
import { ref } from 'vue';
import ButtonChil from './components/ButtonChil.vue';
  function mensagemBotao(texto){
    alert(`O botão clicado foi ${texto}`)
  }
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
    <ButtonChil :nome="'Novo'" :tipo="'btn'" :acao="'btn-novo'" @clique="mensagemBotao">
      Novo
    </ButtonChil>
    <ButtonChil :nome="'Editar'" :tipo="'btn'" :acao="'btn-editar'" @clique="mensagemBotao">
      Editar
    </ButtonChil>
    <ButtonChil :nome="'Salvar'" :tipo="'btn'" :acao="'btn-salvar'" @clique="mensagemBotao">
      Salvar
    </ButtonChil>
    <ButtonChil :nome="'Cancelar'" :acao="'btn-cancelar'" :tipo="'btn'" @clique="mensagemBotao">
      Cancelar
    </ButtonChil>
    <ButtonChil :nome="'Excluir'" :tipo="'btn'" :acao="'btn-excluir'" @clique="mensagemBotao">
      Excluir
    </ButtonChil>

  </div>
</div>
</template>

<style scoped>

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
