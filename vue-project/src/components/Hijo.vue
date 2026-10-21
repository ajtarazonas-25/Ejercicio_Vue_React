<template>
    <div>
        <p>
            Componente visible
        </p>
        <button @click="contador++">Clicks: {{ contador }}</button>
    </div>
</template>
<script setup>
import {ref, onMounted, onUpdated, onUnmounted} from 'vue'
const contador = ref(0)

onMounted(()=> console.log('Montado'))
onUpdated(()=> console.log('Actualizado'))
onUnmounted(()=> console.log('Desmontado'))

</script>
