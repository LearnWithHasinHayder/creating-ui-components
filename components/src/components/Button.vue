<script setup>
// const props = defineProps([
//     'label', 'color'
// ])

const props = defineProps({
    label: {
        type: String,
        default: 'Click Me'
    },
    color: {
        type: String,
        default: 'blue'
    }
})

function getColor(){
    return `bg-${props.color}-500 hover:bg-${props.color}-700`
}
</script>
 
<template>
    <button :class="getColor()" class="text-white font-bold py-2 px-4 rounded">
        {{ label }}
    </button>
</template>
 
<style scoped></style>