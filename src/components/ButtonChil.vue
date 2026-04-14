<script setup>
defineProps(['nome', 'tipo', 'acao'])
</script>
  <template>
<button :class="[tipo, acao]">
  {{ nome }}
</button>
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

</style>
