<script setup>
import { reactive } from 'vue';
const menulist = [
    'camisetas',
    'acessórios',
    'quadros'
]

const state = reactive({ isactive: false })

function handleMenu() {
    state.isactive = !state.isactive
}


</script>

<template>
    
</template>



