<script setup>
import App from '@/App.vue';
defineProps(['nome', 'tipo', 'acao'])
defineEmits(['clique'])
</script>
  <template>
<button :class="[tipo, acao]" @click.prevent="$emit('clique', nome)">
  <slot>

  </slot>
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

</style>
