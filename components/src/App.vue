<script setup>
import Button from './components/Button.vue'
import ButtonCounter from './components/ButtonCounter.vue'
import Location from './components/Location.vue'

const data = [
  {
    image:"https://images.unsplash.com/photo-1615319532762-b4ccc69e5abf?ixid=MXwxMjA3fDB8MHxzZWFyY2h8MTA3fHxsYW5kc2NhcGV8ZW58MHx8MHw%3D&amp;ixlib=rb-1.2.1&amp;auto=format&amp;fit=crop&amp;w=900&amp;q=100",
    location:"California",
    price:87,
    rating:4,
    time:15,
    title:"Photo by Drew Dao",
  },
  {
    image:"https://images.unsplash.com/photo-1562981943-dda9d14477f0?ixid=MXwxMjA3fDB8MHxzZWFyY2h8MTE4fHxsYW5kc2NhcGV8ZW58MHx8MHw%3D&amp;ixlib=rb-1.2.1&amp;auto=format&amp;fit=crop&amp;w=900&amp;q=100",
    location:"San Diego, California",
    price:75,
    rating:4,
    time:21,
    title:"Photo by Trent Haaland",
  }
]
</script>

<template>
  <div class="container mx-auto">
    <div class="flex items-center mt-5">
      <img class="logo" src="./assets/vue.svg" alt="Vue logo" />
      <h1 class="text-2xl">Vue Components</h1>
    </div>
    <section class="p-10 md:py-20 px-5 ">
      <section class="flex space-x-10">

        <!-- <Location v-for="item in data" :key="item.title" :image="item.image" :location="item.location" :price="item.price" :rating="item.rating" :time="item.time" :title="item.title" /> -->
        <Location v-for="item in data" :key="item.title" v-bind="item" />

      </section>

    </section>

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
