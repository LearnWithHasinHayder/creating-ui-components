<script setup>
const props = defineProps([
    'image', 'location', 'price', 'rating', 'time', 'title'
])

</script>
 
<template>
    <article class=" pb-5 max-w-sm transform duration-500 hover:-translate-y-1 cursor-pointer group">
        <div class="max-h-125 overflow-hidden">
            <img class="transform duration-300 group-hover:scale-110" :src="image" alt="">
        </div>
        <div class="flex justify-between my-5 ">
            <div class="text-orange-500 text-base font-semibold"> {{ location }}</div>
            <div class="text-base text-right"><span class="font-bold">{{ price }}</span>/Day</div>
        </div>
        <h2 class="font-bold text-2xl"> {{ title }}</h2>
        <div class="flex justify-between items-center mt-3 ">
            <div class="text-base uppercase font-semibold text-gray-500">{{ time }} Days Tour</div>
            <div class="text-base text-right">
                <div class="flex">
                    <svg v-for="index in rating" :key="index" class="w-4 h-4 mx-px fill-current text-orange-600" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 14 14">
                        <path d="M6.43 12l-2.36 1.64a1 1 0 0 1-1.53-1.11l.83-2.75a1 1 0 0 0-.35-1.09L.73 6.96a1 1 0 0 1 .59-1.8l2.87-.06a1 1 0 0 0 .92-.67l.95-2.71a1 1 0 0 1 1.88 0l.95 2.71c.13.4.5.66.92.67l2.87.06a1 1 0 0 1 .59 1.8l-2.3 1.73a1 1 0 0 0-.34 1.09l.83 2.75a1 1 0 0 1-1.53 1.1L7.57 12a1 1 0 0 0-1.14 0z"></path>
                    </svg>
                </div>
            </div>
        </div>
    </article>
</template>
 
<style scoped></style>