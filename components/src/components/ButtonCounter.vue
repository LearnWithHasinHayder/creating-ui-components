<script setup>
import {ref} from 'vue'

const props = defineProps({
    count: {
        type: Number,
        default: 0
    },
})

const counter = ref(props.count)

function increase(){
    counter.value++
}

function decrease(){
    counter.value--
}
</script>
 
<template>
    <button @click="increase()" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        +
    </button>
    <span class="px-5"> 
        {{ counter }} 
    </span>
    <button @click="decrease()" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        -
    </button>
</template>
 
<style scoped></style>