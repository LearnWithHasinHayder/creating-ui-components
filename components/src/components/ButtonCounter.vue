<script setup>
import {ref} from 'vue'
const count = ref(0)

function increase(){
    count.value++
}

function decrease(){
    count.value--
}
</script>
 
<template>
    <button @click="increase()" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        +
    </button>
    <span class="px-5"> 
        {{ count }} 
    </span>
    <button @click="decrease()" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        -
    </button>
</template>
 
<style scoped></style>