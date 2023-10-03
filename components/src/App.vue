<script setup>
</script>

<template>
  <div class="container mx-auto">
    <div class="flex items-center mt-5">
      <img class="logo" src="./assets/vue.svg" alt="Vue logo" />
      <h1 class="text-2xl">Vue Components</h1>
    </div>
    <div class="mt-10 p-10">
      <p class="mb-3">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis corporis mollitia fugit dolor quibusdam atque qui fuga laudantium aut porro.
      </p>
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        Button
      </button>
      <Button color="orange" label="Click me"/>
    </div>
    
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
