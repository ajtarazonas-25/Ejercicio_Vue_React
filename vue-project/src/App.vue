<template>
  <div style = "text-align:center; margin-top:50px;">
    <h2>Ejercicio 1: Vue 3 Logs</h2>
    
    <button @click="mostrar = !mostrar" style="margin-left:10px;"> {{ mostrar ? 'Ocultar' : 'Mostrar' }} componente</button>

    <Hijo v-if="mostrar" />
  </div>
</template>
<script setup>
import { ref} from 'vue'
import Hijo from './components/Hijo.vue'

const mostrar = ref(true)
</script>
