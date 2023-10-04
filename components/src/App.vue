<script setup>
import Button from './components/Button.vue'
import ButtonCounter from './components/ButtonCounter.vue'
import Location from './components/Location.vue'
import ApplicantDetails from './components/ApplicantDetails.vue'
const people = [
  {
    name:'Margot Foster',
    position:'Backend Developer',
    email:'margotfoster@example.com',
    salary:'$120,000',
    about:'Fugiat ipsum ipsum deserunt culpa aute sint do nostrud anim incididunt cillum culpa consequat. Excepteur qui ipsum aliquip consequat sint. Sit id mollit nulla mollit nostrud in ea officia proident. Irure nostrud pariatur mollit ad adipisicing reprehenderit deserunt qui eu.',
    attachments:[
      {
        name:'resume_back_end_developer.pdf',
        size:'256kb',
        type:'PDF',
        url:'#'
      },
      {
        name:'coverletter_back_end_developer.pdf',
        size:'128kb',
        type:'PDF',
        url:'#'
      }
    ]
  },
  {
    name:'John Doe',
    position:'Frontend Developer',
    email:'john@doe.com',
    salary:'$100,000',
    about:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.',
    attachments:[
      {
        name:'resume_front_end_developer.pdf',
        size:'1MB',
        type:'PDF',
        url:'#'
      },
      {
        name:'coverletter_front_end_developer.pdf',
        size:'512kb',
        type:'PDF',
        url:'#'
      }
    ]
  },
  {
    name:'Jane Doe',
    position:'Designer',
    email:'jane@doe.com',
    salary:'$110,000',
    about:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum. Here is some more text.',
    attachments:[
      {
        name:'resume_designer.pdf',
        size:'5MB',
        type:'PDF',
        url:'#'
      },
      {
        name:'coverletter_designer.pdf',
        size:'2MB',
        type:'PDF',
        url:'#'
      }
    ]
  }
]
</script>

<template>
  <div class="container mx-auto">
    <div class="flex items-center mt-5">
      <img class="logo" src="./assets/vue.svg" alt="Vue logo" />
      <h1 class="text-2xl">Vue Components</h1>
    </div>
    <section class="mx-auto mt-10">
      <ApplicantDetails :applicants="people"/>
  </section>

</div></template>

<style scoped>.logo {
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
}</style>
